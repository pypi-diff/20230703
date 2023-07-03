# Comparing `tmp/sqlalchemy_bind_manager-0.3.1.tar.gz` & `tmp/sqlalchemy_bind_manager-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_bind_manager-0.3.1.tar", max compression
+gzip compressed data, was "sqlalchemy_bind_manager-0.3.2.tar", max compression
```

## Comparing `sqlalchemy_bind_manager-0.3.1.tar` & `sqlalchemy_bind_manager-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/LICENSE
--rw-r--r--   0        0        0    11983 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/README.md
--rw-r--r--   0        0        0     2244 2023-06-24 15:01:03.217054 sqlalchemy_bind_manager-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      107 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/__init__.py
--rw-r--r--   0        0        0     5241 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_bind_manager.py
--rw-r--r--   0        0        0      197 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/__init__.py
--rw-r--r--   0        0        0     5734 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/async_.py
--rw-r--r--   0        0        0    11340 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/base_repository.py
--rw-r--r--   0        0        0     1099 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/common.py
--rw-r--r--   0        0        0     7429 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/result_presenters.py
--rw-r--r--   0        0        0     5045 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/sync.py
--rw-r--r--   0        0        0     3125 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_transaction_handler.py
--rw-r--r--   0        0        0     1722 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_unit_of_work.py
--rw-r--r--   0        0        0      310 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/exceptions.py
--rw-r--r--   0        0        0    10397 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/protocols.py
--rw-r--r--   0        0        0        0 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/py.typed
--rw-r--r--   0        0        0      242 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/repository.py
--rw-r--r--   0        0        0    13376 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-03 10:48:06.193385 sqlalchemy_bind_manager-0.3.2/LICENSE
+-rw-r--r--   0        0        0     8733 2023-07-03 10:48:06.193385 sqlalchemy_bind_manager-0.3.2/README.md
+-rw-r--r--   0        0        0     2375 2023-07-03 10:48:24.013456 sqlalchemy_bind_manager-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/__init__.py
+-rw-r--r--   0        0        0     5241 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_bind_manager.py
+-rw-r--r--   0        0        0      197 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/__init__.py
+-rw-r--r--   0        0        0     5734 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/async_.py
+-rw-r--r--   0        0        0    11340 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/base_repository.py
+-rw-r--r--   0        0        0     1099 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/common.py
+-rw-r--r--   0        0        0     7429 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/result_presenters.py
+-rw-r--r--   0        0        0     5045 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/sync.py
+-rw-r--r--   0        0        0     3229 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_transaction_handler.py
+-rw-r--r--   0        0        0     1722 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_unit_of_work/__init__.py
+-rw-r--r--   0        0        0      310 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/exceptions.py
+-rw-r--r--   0        0        0    10397 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/protocols.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/py.typed
+-rw-r--r--   0        0        0      242 2023-07-03 10:48:06.197385 sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/repository.py
+-rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.3.2/PKG-INFO
```

### Comparing `sqlalchemy_bind_manager-0.3.1/LICENSE` & `sqlalchemy_bind_manager-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.1/README.md` & `sqlalchemy_bind_manager-0.3.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: sqlalchemy-bind-manager
+Version: 0.3.2
+Summary: A manager to easily handle multiple SQLAlchemy configurations
+Home-page: https://febus982.github.io/sqlalchemy-bind-manager
+License: MIT
+Keywords: sqlalchemy,config,manager
+Author: Federico Busetti
+Author-email: 729029+febus982@users.noreply.github.com
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: AsyncIO
+Classifier: Framework :: Pydantic
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Database
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: SQLAlchemy[asyncio,mypy] (>=2.0.0,<2.1.0)
+Requires-Dist: pydantic (>=1.10.2,<1.11.0)
+Project-URL: Repository, https://github.com/febus982/sqlalchemy-bind-manager
+Description-Content-Type: text/markdown
+
 # SQLAlchemy bind manager
 [![Stable Version](https://img.shields.io/pypi/v/sqlalchemy-bind-manager?color=blue)](https://pypi.org/project/sqlalchemy-bind-manager/)
 [![stability-beta](https://img.shields.io/badge/stability-beta-33bbff.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#beta)
 
 [![Python 3.8](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.8.yml/badge.svg?event=push)](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.8.yml)
 [![Python 3.9](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.9.yml/badge.svg?event=push)](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.9.yml)
 [![Python 3.10](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.10.yml/badge.svg?event=push)](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.10.yml)
@@ -27,16 +60,20 @@
 pip install sqlalchemy-bind-manager
 ```
 
 ## Components maturity
 
 [//]: # (https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md)
 * [![stability-beta](https://img.shields.io/badge/stability-beta-33bbff.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#beta) **SQLAlchemy manager:** Implementation is mostly finalised, needs testing in production.
-* [![stability-beta](https://img.shields.io/badge/stability-beta-33bbff.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#beta) **Repository / Unit of work:** Implementation is mostly finalised, needs testing in production.
+* [![stability-beta](https://img.shields.io/badge/stability-beta-33bbff.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#beta) **Repository:** Implementation is mostly finalised, needs testing in production.
+* [![stability-experimental](https://img.shields.io/badge/stability-experimental-orange.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#experimental) **Unit of work:** The implementation is working but limited to repositories using the same engine. Distributed transactions across different engines are not yet supported.
+
+## Documentation
 
+The complete documentation can be found [here](https://febus982.github.io/sqlalchemy-bind-manager)
 
 ## SQLAlchemy manager 
 
 Initialise the manager providing an instance of `SQLAlchemyConfig`
 
 ```python
 from sqlalchemy_bind_manager import SQLAlchemyConfig, SQLAlchemyBindManager
@@ -46,74 +83,46 @@
     engine_options=dict(connect_args={"check_same_thread": False}, echo=True),
     session_options=dict(expire_on_commit=False),
 )
 
 sa_manager = SQLAlchemyBindManager(config)
 ```
 
-🚨 NOTE: Using global variables is not thread-safe, please read the [Threading](#threading) section if your application uses multi-threading.
+🚨 NOTE: Using global variables is not thread-safe, please read the [Documentation](https://febus982.github.io/sqlalchemy-bind-manager/manager/session/#note-on-multithreaded-applications) if your application uses multi-threading.
 
 The `engine_url` and `engine_options` dictionaries accept the same parameters as SQLAlchemy [create_engine()](https://docs.sqlalchemy.org/en/14/core/engines.html#sqlalchemy.create_engine)
 
 The `session_options` dictionary accepts the same parameters as SQLALchemy [sessionmaker()](https://docs.sqlalchemy.org/en/14/orm/session_api.html#sqlalchemy.orm.sessionmaker)
 
-Once the bind manager is initialised we can retrieve and use the SQLAlchemyBind using the method `get_bind()`
-
-The `SQLAlchemyBind` and `SQLAlchemyAsyncBind` class has the following attributes:
-
-* `engine`: The initialised SQLALchemy `Engine`
-* `model_declarative_base`: A base class that can be used to create [declarative models](https://docs.sqlalchemy.org/en/14/orm/mapping_styles.html#declarative-mapping)
-* `registry_mapper`: The `registry` associated with the `engine`. It can be used with Alembic or to setup [imperative mapping](https://docs.sqlalchemy.org/en/14/orm/mapping_styles.html#imperative-mapping)
-* `session_class`: The class built by [sessionmaker()](https://docs.sqlalchemy.org/en/14/orm/session_api.html#sqlalchemy.orm.sessionmaker), either `Session` or `AsyncSession`
-
-The `SQLAlchemyBindManager` provides some helper methods to quickly access some of the bind properties without using the `SQLAlchemyBind`:
+The `SQLAlchemyBindManager` provides some helper methods for common operations:
 
-* `get_session`: returns a Session object
+* `get_bind`: returns a `SQLAlchemyBind` or `SQLAlchemyAsyncBind` object
+* `get_session`: returns a `Session` object, which works also as a context manager
 * `get_mapper`: returns the mapper associated with the bind
 
 Example:
 
 ```python
 bind = sa_manager.get_bind()
 
 
-class DeclarativeModel(bind.model_declarative_base):
+class MyModel(bind.model_declarative_base):
     pass
 
 
-class ImperativeModel:
-    id: int
-
-
-imperative_table = Table(
-    "imperative",
-    bind.registry_mapper.metadata,
-    Column("id", Integer, primary_key=True),
-    Column("name", String, primary_key=True),
-)
-
-bind.registry_mapper.map_imperatively(ImperativeModel, imperative_table)
-
-# or using the get_mapper() helper method
-sa_manager.get_mapper().map_imperatively(ImperativeModel, imperative_table)
-
 # Persist an object
-o = ImperativeModel()  # also o = DeclarativeModel()
+o = MyModel()
 o.name = "John"
-with sa_manager.get_bind().session_class()() as session:
-    session.add(o)
-    session.commit()
-
-# or using the get_session() helper method for better readability
 with sa_manager.get_session() as session:
     session.add(o)
     session.commit()
-
 ```
 
+[Imperative model declaration](https://febus982.github.io/sqlalchemy-bind-manager/manager/models/) is also supported.
+
 ### Multiple database binds
 
 `SQLAlchemyBindManager` accepts also multiple databases configuration, provided as a dictionary. The dictionary keys are used as a reference name for each bind.
 
 ```python
 from sqlalchemy_bind_manager import SQLAlchemyConfig, SQLAlchemyBindManager
 
@@ -131,56 +140,29 @@
 }
 
 sa_manager = SQLAlchemyBindManager(config)
 ```
 
 All the `SQLAlchemyBindManager` helper methods accept the `bind_name` optional parameter:
 
-* `get_session(bind_name="default")`: returns a `Session` or `AsyncSession` object
+* `get_bind(bind_name="default")`: returns a `SQLAlchemyBind` or `SQLAlchemyAsyncBind` object
+* `get_session(bind_name="default")`: returns a `Session` or `AsyncSession` object, which works also as a context manager
 * `get_mapper(bind_name="default")`: returns the mapper associated with the bind
 
-### Threading
-
-Global variables are shared between different threads in python. If your application uses
-multiple threads, like spawning a thread per request, then you should not store an
-initialised session in a global variable, otherwise the state of your models will be shared
-among the threads and produce undesired changes in the database.
-
-This is not thread safe:
-
-```python
-session = sa_manager.get_session()
-session.add(model)
-session.commit()
-```
-
-If you truly need to have a long-lived session you'll need to use a scoped session,
-something like this:
-
-```python
-from sqlalchemy.orm import scoped_session
-
-session = scoped_session(sa_manager.get_bind().session_class())
-```
-
-Handling the life cycle of scoped sessions is not supported by this documentations.
-Please refer to [SQLAlchemy documentation](https://docs.sqlalchemy.org/en/20/orm/contextual.html)
-about this.
-
 ### Asynchronous database binds
 
 Is it possible to supply configurations for asyncio supported engines.
 
 ```python
 config = SQLAlchemyAsyncConfig(
     engine_url="postgresql+asyncpg://scott:tiger@localhost/test",
 )
 ```
 
-This will make sure we have an `AsyncEngine` and an `AsyncSession` are initialised.
+This will make sure we have an `AsyncEngine` and an `AsyncSession` are initialised, as an asynchronous context manager.
 
 ```python
 async with sa_manager.get_session() as session:
     session.add(o)
     session.commit()
 ```
 
@@ -207,53 +189,24 @@
     def _some_custom_method_implemented(self):
         ...
 
 # Extended class usage
 extended_repo_instance = ModelRepository(sqlalchemy_bind_manager.get_bind())
 ```
 
-The classes provide some common use methods:
+The repository classes provides methods for  common use case:
 
-* `get`: Retrieve a model by identifier
+* `get`: Retrieve a model by primary key
 * `save`: Persist a model
 * `save_many`: Persist multiple models in a single transaction
 * `delete`: Delete a model
 * `find`: Search for a list of models (basically an adapter for SELECT queries)
 * `paginated_find`: Search for a list of models, with pagination support
 * `cursor_paginated_find`: Search for a list of models, with cursor based pagination support
 
-### Session lifecycle in repositories
-
-[SQLAlchemy documentation](https://docs.sqlalchemy.org/en/20/orm/session_basics.html#when-do-i-construct-a-session-when-do-i-commit-it-and-when-do-i-close-it)
-recommends we create `Session` object at the beginning of a logical operation where
-database access is potentially anticipated.
-
-Doing this too soon might cause unexpected effects, like unexpected updates being committed,
-if the initialised session is shared among different repositories.
-
-A `Repository` represents a generic interface to persist data object to a storage, not necessarily
-using SQLAlchemy. It makes sense that the lifecycle of a `Session` follows the one of the Repository
-(The assumption is: if we create a Repository, we're going to do a DB operation,
-otherwise we wouldn't need one).
-
-Each Repository instance create an internal scoped session. The session gets
-automatically closed when the Repository instance is not referenced by any variable (and the
-garbage collector clean it up)
-
-In this way we ensure the `Session` we use is isolated, and the same for all the operations we do with the
-same Repository. 
-
-This approach has a consequence: We can't use SQLAlchemy lazy loading, so we'll need to make sure relationship are always loaded eagerly,
-using either approach:
-* Setup your model/table relationships to always use always eager loading
-* Implement ad-hoc methods to deal with relationships as necessary
-
-Note that `AsyncSession` has [the same limitation on lazy loading](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html#asyncio-orm-avoid-lazyloads),
-even when keeping the session opened, so it makes sense that the two Repository implementations behave consistently.
-
 ### Use the Unit Of Work to share a session among multiple repositories
 
 It is possible we need to run several operations in a single database transaction. While a single
 repository provide by itself an isolated session for single operations, we have to use a different
 approach for multiple operations.
 
 We can use the `UnitOfWork` or the `AsyncUnitOfWork` class to provide a shared session to
@@ -267,13 +220,9 @@
 
 bind = sa_manager.get_bind()
 uow = UnitOfWork(bind, (MyRepo, MyOtherRepo))
 
 with uow.transaction():
     uow.MyRepo.save(some_model)
     uow.MyOtherRepo.save(some_other_model)
-
-# Optionally disable the commit/rollback handling
-with uow.transaction(read_only=True):
-    model1 = uow.MyRepo.get(1)
-    model2 = uow.MyOtherRepo.get(2)
 ```
+
```

### Comparing `sqlalchemy_bind_manager-0.3.1/pyproject.toml` & `sqlalchemy_bind_manager-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy-bind-manager"
-version = "0.3.1"
+version = "0.3.2"
 description = "A manager to easily handle multiple SQLAlchemy configurations"
 license = "MIT"
 authors = ["Federico Busetti <729029+febus982@users.noreply.github.com>"]
 repository = "https://github.com/febus982/sqlalchemy-bind-manager"
 homepage = "https://febus982.github.io/sqlalchemy-bind-manager"
 readme = "README.md"
 packages = [{include = "sqlalchemy_bind_manager"}]
@@ -70,11 +70,25 @@
 
 [tool.mypy]
 files = "sqlalchemy_bind_manager"
 plugins = "pydantic.mypy"
 
 [tool.ruff]
 select = ["E", "F", "I"]
+extend-exclude = ["docs"]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 "repository.py" = ["F401"]
+
+[tool.black]
+files = '''
+(
+  sqlalchemy_bind_manager
+  tests
+)
+'''
+extend-exclude = '''
+(
+  /docs
+)
+'''
```

### Comparing `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_bind_manager.py` & `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_bind_manager.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/async_.py` & `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/async_.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/base_repository.py` & `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/base_repository.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/common.py` & `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/common.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/result_presenters.py` & `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/result_presenters.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/sync.py` & `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_repository/sync.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_transaction_handler.py` & `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_transaction_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from asyncio import get_event_loop
+import asyncio
 from contextlib import asynccontextmanager, contextmanager
 from typing import AsyncIterator, Iterator
 from uuid import uuid4
 
 from sqlalchemy.ext.asyncio import (
     AsyncSession,
     async_scoped_session,
@@ -70,19 +70,22 @@
             )
             self.session = self._session_class()
 
     def __del__(self):
         if not getattr(self, "_session_class", None):
             return
 
-        loop = get_event_loop()
-        if loop.is_running():
-            loop.create_task(self._session_class.remove())
-        else:
-            loop.run_until_complete(self._session_class.remove())
+        try:
+            loop = asyncio.get_event_loop()
+            if loop.is_running():
+                loop.create_task(self._session_class.remove())
+            else:
+                loop.run_until_complete(self._session_class.remove())
+        except RuntimeError:
+            asyncio.run(self._session_class.remove())
 
     @asynccontextmanager
     async def get_session(self, read_only: bool = False) -> AsyncIterator[AsyncSession]:
         try:
             await self.session.begin()
             yield self.session
             if not read_only:
```

### Comparing `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_unit_of_work.py` & `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/_unit_of_work/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/protocols.py` & `sqlalchemy_bind_manager-0.3.2/sqlalchemy_bind_manager/protocols.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.1/PKG-INFO` & `sqlalchemy_bind_manager-0.3.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: sqlalchemy-bind-manager
-Version: 0.3.1
-Summary: A manager to easily handle multiple SQLAlchemy configurations
-Home-page: https://febus982.github.io/sqlalchemy-bind-manager
-License: MIT
-Keywords: sqlalchemy,config,manager
-Author: Federico Busetti
-Author-email: 729029+febus982@users.noreply.github.com
-Requires-Python: >=3.8,<3.12
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: AsyncIO
-Classifier: Framework :: Pydantic
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Database
-Classifier: Topic :: Database :: Front-Ends
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed
-Requires-Dist: SQLAlchemy[asyncio,mypy] (>=2.0.0,<2.1.0)
-Requires-Dist: pydantic (>=1.10.2,<1.11.0)
-Project-URL: Repository, https://github.com/febus982/sqlalchemy-bind-manager
-Description-Content-Type: text/markdown
-
 # SQLAlchemy bind manager
 [![Stable Version](https://img.shields.io/pypi/v/sqlalchemy-bind-manager?color=blue)](https://pypi.org/project/sqlalchemy-bind-manager/)
 [![stability-beta](https://img.shields.io/badge/stability-beta-33bbff.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#beta)
 
 [![Python 3.8](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.8.yml/badge.svg?event=push)](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.8.yml)
 [![Python 3.9](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.9.yml/badge.svg?event=push)](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.9.yml)
 [![Python 3.10](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.10.yml/badge.svg?event=push)](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.10.yml)
@@ -60,16 +27,20 @@
 pip install sqlalchemy-bind-manager
 ```
 
 ## Components maturity
 
 [//]: # (https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md)
 * [![stability-beta](https://img.shields.io/badge/stability-beta-33bbff.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#beta) **SQLAlchemy manager:** Implementation is mostly finalised, needs testing in production.
-* [![stability-beta](https://img.shields.io/badge/stability-beta-33bbff.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#beta) **Repository / Unit of work:** Implementation is mostly finalised, needs testing in production.
+* [![stability-beta](https://img.shields.io/badge/stability-beta-33bbff.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#beta) **Repository:** Implementation is mostly finalised, needs testing in production.
+* [![stability-experimental](https://img.shields.io/badge/stability-experimental-orange.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#experimental) **Unit of work:** The implementation is working but limited to repositories using the same engine. Distributed transactions across different engines are not yet supported.
+
+## Documentation
 
+The complete documentation can be found [here](https://febus982.github.io/sqlalchemy-bind-manager)
 
 ## SQLAlchemy manager 
 
 Initialise the manager providing an instance of `SQLAlchemyConfig`
 
 ```python
 from sqlalchemy_bind_manager import SQLAlchemyConfig, SQLAlchemyBindManager
@@ -79,74 +50,46 @@
     engine_options=dict(connect_args={"check_same_thread": False}, echo=True),
     session_options=dict(expire_on_commit=False),
 )
 
 sa_manager = SQLAlchemyBindManager(config)
 ```
 
-🚨 NOTE: Using global variables is not thread-safe, please read the [Threading](#threading) section if your application uses multi-threading.
+🚨 NOTE: Using global variables is not thread-safe, please read the [Documentation](https://febus982.github.io/sqlalchemy-bind-manager/manager/session/#note-on-multithreaded-applications) if your application uses multi-threading.
 
 The `engine_url` and `engine_options` dictionaries accept the same parameters as SQLAlchemy [create_engine()](https://docs.sqlalchemy.org/en/14/core/engines.html#sqlalchemy.create_engine)
 
 The `session_options` dictionary accepts the same parameters as SQLALchemy [sessionmaker()](https://docs.sqlalchemy.org/en/14/orm/session_api.html#sqlalchemy.orm.sessionmaker)
 
-Once the bind manager is initialised we can retrieve and use the SQLAlchemyBind using the method `get_bind()`
-
-The `SQLAlchemyBind` and `SQLAlchemyAsyncBind` class has the following attributes:
-
-* `engine`: The initialised SQLALchemy `Engine`
-* `model_declarative_base`: A base class that can be used to create [declarative models](https://docs.sqlalchemy.org/en/14/orm/mapping_styles.html#declarative-mapping)
-* `registry_mapper`: The `registry` associated with the `engine`. It can be used with Alembic or to setup [imperative mapping](https://docs.sqlalchemy.org/en/14/orm/mapping_styles.html#imperative-mapping)
-* `session_class`: The class built by [sessionmaker()](https://docs.sqlalchemy.org/en/14/orm/session_api.html#sqlalchemy.orm.sessionmaker), either `Session` or `AsyncSession`
-
-The `SQLAlchemyBindManager` provides some helper methods to quickly access some of the bind properties without using the `SQLAlchemyBind`:
+The `SQLAlchemyBindManager` provides some helper methods for common operations:
 
-* `get_session`: returns a Session object
+* `get_bind`: returns a `SQLAlchemyBind` or `SQLAlchemyAsyncBind` object
+* `get_session`: returns a `Session` object, which works also as a context manager
 * `get_mapper`: returns the mapper associated with the bind
 
 Example:
 
 ```python
 bind = sa_manager.get_bind()
 
 
-class DeclarativeModel(bind.model_declarative_base):
+class MyModel(bind.model_declarative_base):
     pass
 
 
-class ImperativeModel:
-    id: int
-
-
-imperative_table = Table(
-    "imperative",
-    bind.registry_mapper.metadata,
-    Column("id", Integer, primary_key=True),
-    Column("name", String, primary_key=True),
-)
-
-bind.registry_mapper.map_imperatively(ImperativeModel, imperative_table)
-
-# or using the get_mapper() helper method
-sa_manager.get_mapper().map_imperatively(ImperativeModel, imperative_table)
-
 # Persist an object
-o = ImperativeModel()  # also o = DeclarativeModel()
+o = MyModel()
 o.name = "John"
-with sa_manager.get_bind().session_class()() as session:
-    session.add(o)
-    session.commit()
-
-# or using the get_session() helper method for better readability
 with sa_manager.get_session() as session:
     session.add(o)
     session.commit()
-
 ```
 
+[Imperative model declaration](https://febus982.github.io/sqlalchemy-bind-manager/manager/models/) is also supported.
+
 ### Multiple database binds
 
 `SQLAlchemyBindManager` accepts also multiple databases configuration, provided as a dictionary. The dictionary keys are used as a reference name for each bind.
 
 ```python
 from sqlalchemy_bind_manager import SQLAlchemyConfig, SQLAlchemyBindManager
 
@@ -164,56 +107,29 @@
 }
 
 sa_manager = SQLAlchemyBindManager(config)
 ```
 
 All the `SQLAlchemyBindManager` helper methods accept the `bind_name` optional parameter:
 
-* `get_session(bind_name="default")`: returns a `Session` or `AsyncSession` object
+* `get_bind(bind_name="default")`: returns a `SQLAlchemyBind` or `SQLAlchemyAsyncBind` object
+* `get_session(bind_name="default")`: returns a `Session` or `AsyncSession` object, which works also as a context manager
 * `get_mapper(bind_name="default")`: returns the mapper associated with the bind
 
-### Threading
-
-Global variables are shared between different threads in python. If your application uses
-multiple threads, like spawning a thread per request, then you should not store an
-initialised session in a global variable, otherwise the state of your models will be shared
-among the threads and produce undesired changes in the database.
-
-This is not thread safe:
-
-```python
-session = sa_manager.get_session()
-session.add(model)
-session.commit()
-```
-
-If you truly need to have a long-lived session you'll need to use a scoped session,
-something like this:
-
-```python
-from sqlalchemy.orm import scoped_session
-
-session = scoped_session(sa_manager.get_bind().session_class())
-```
-
-Handling the life cycle of scoped sessions is not supported by this documentations.
-Please refer to [SQLAlchemy documentation](https://docs.sqlalchemy.org/en/20/orm/contextual.html)
-about this.
-
 ### Asynchronous database binds
 
 Is it possible to supply configurations for asyncio supported engines.
 
 ```python
 config = SQLAlchemyAsyncConfig(
     engine_url="postgresql+asyncpg://scott:tiger@localhost/test",
 )
 ```
 
-This will make sure we have an `AsyncEngine` and an `AsyncSession` are initialised.
+This will make sure we have an `AsyncEngine` and an `AsyncSession` are initialised, as an asynchronous context manager.
 
 ```python
 async with sa_manager.get_session() as session:
     session.add(o)
     session.commit()
 ```
 
@@ -240,53 +156,24 @@
     def _some_custom_method_implemented(self):
         ...
 
 # Extended class usage
 extended_repo_instance = ModelRepository(sqlalchemy_bind_manager.get_bind())
 ```
 
-The classes provide some common use methods:
+The repository classes provides methods for  common use case:
 
-* `get`: Retrieve a model by identifier
+* `get`: Retrieve a model by primary key
 * `save`: Persist a model
 * `save_many`: Persist multiple models in a single transaction
 * `delete`: Delete a model
 * `find`: Search for a list of models (basically an adapter for SELECT queries)
 * `paginated_find`: Search for a list of models, with pagination support
 * `cursor_paginated_find`: Search for a list of models, with cursor based pagination support
 
-### Session lifecycle in repositories
-
-[SQLAlchemy documentation](https://docs.sqlalchemy.org/en/20/orm/session_basics.html#when-do-i-construct-a-session-when-do-i-commit-it-and-when-do-i-close-it)
-recommends we create `Session` object at the beginning of a logical operation where
-database access is potentially anticipated.
-
-Doing this too soon might cause unexpected effects, like unexpected updates being committed,
-if the initialised session is shared among different repositories.
-
-A `Repository` represents a generic interface to persist data object to a storage, not necessarily
-using SQLAlchemy. It makes sense that the lifecycle of a `Session` follows the one of the Repository
-(The assumption is: if we create a Repository, we're going to do a DB operation,
-otherwise we wouldn't need one).
-
-Each Repository instance create an internal scoped session. The session gets
-automatically closed when the Repository instance is not referenced by any variable (and the
-garbage collector clean it up)
-
-In this way we ensure the `Session` we use is isolated, and the same for all the operations we do with the
-same Repository. 
-
-This approach has a consequence: We can't use SQLAlchemy lazy loading, so we'll need to make sure relationship are always loaded eagerly,
-using either approach:
-* Setup your model/table relationships to always use always eager loading
-* Implement ad-hoc methods to deal with relationships as necessary
-
-Note that `AsyncSession` has [the same limitation on lazy loading](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html#asyncio-orm-avoid-lazyloads),
-even when keeping the session opened, so it makes sense that the two Repository implementations behave consistently.
-
 ### Use the Unit Of Work to share a session among multiple repositories
 
 It is possible we need to run several operations in a single database transaction. While a single
 repository provide by itself an isolated session for single operations, we have to use a different
 approach for multiple operations.
 
 We can use the `UnitOfWork` or the `AsyncUnitOfWork` class to provide a shared session to
@@ -300,14 +187,8 @@
 
 bind = sa_manager.get_bind()
 uow = UnitOfWork(bind, (MyRepo, MyOtherRepo))
 
 with uow.transaction():
     uow.MyRepo.save(some_model)
     uow.MyOtherRepo.save(some_other_model)
-
-# Optionally disable the commit/rollback handling
-with uow.transaction(read_only=True):
-    model1 = uow.MyRepo.get(1)
-    model2 = uow.MyOtherRepo.get(2)
 ```
-
```


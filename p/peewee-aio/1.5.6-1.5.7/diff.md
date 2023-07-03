# Comparing `tmp/peewee_aio-1.5.6.tar.gz` & `tmp/peewee_aio-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_aio-1.5.6.tar", max compression
+gzip compressed data, was "peewee_aio-1.5.7.tar", max compression
```

## Comparing `peewee_aio-1.5.6.tar` & `peewee_aio-1.5.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4681 2023-06-23 06:25:39.878860 peewee_aio-1.5.6/README.md
--rw-r--r--   0        0        0      132 2023-06-23 06:25:39.878860 peewee_aio-1.5.6/peewee_aio/__init__.py
--rw-r--r--   0        0        0     1210 2023-06-23 06:25:39.878860 peewee_aio-1.5.6/peewee_aio/databases.py
--rw-r--r--   0        0        0    17336 2023-06-23 06:25:39.878860 peewee_aio-1.5.6/peewee_aio/fields.py
--rw-r--r--   0        0        0    15580 2023-06-23 06:25:39.878860 peewee_aio-1.5.6/peewee_aio/manager.py
--rw-r--r--   0        0        0    16692 2023-06-23 06:25:39.878860 peewee_aio-1.5.6/peewee_aio/model.py
--rw-r--r--   0        0        0        0 2023-06-23 06:25:39.878860 peewee_aio-1.5.6/peewee_aio/py.typed
--rw-r--r--   0        0        0      268 2023-06-23 06:25:39.882861 peewee_aio-1.5.6/peewee_aio/types.py
--rw-r--r--   0        0        0     2622 2023-06-23 06:25:39.882861 peewee_aio-1.5.6/pyproject.toml
--rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 peewee_aio-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0     4681 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/README.md
+-rw-r--r--   0        0        0      132 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/__init__.py
+-rw-r--r--   0        0        0     1210 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/databases.py
+-rw-r--r--   0        0        0    17336 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/fields.py
+-rw-r--r--   0        0        0    15580 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/manager.py
+-rw-r--r--   0        0        0    17014 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/model.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/py.typed
+-rw-r--r--   0        0        0      268 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/types.py
+-rw-r--r--   0        0        0     2622 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/pyproject.toml
+-rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 peewee_aio-1.5.7/PKG-INFO
```

### Comparing `peewee_aio-1.5.6/README.md` & `peewee_aio-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.6/peewee_aio/databases.py` & `peewee_aio-1.5.7/peewee_aio/databases.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.6/peewee_aio/fields.py` & `peewee_aio-1.5.7/peewee_aio/fields.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.6/peewee_aio/manager.py` & `peewee_aio-1.5.7/peewee_aio/manager.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.6/peewee_aio/model.py` & `peewee_aio-1.5.7/peewee_aio/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,19 @@
         meta = cls._meta
         if getattr(cls, "_manager", None) and not meta.database:
             meta.database = cls._manager.pw_database
 
         return cls
 
 
+class AIOModelAlias(ModelAlias, Generic[TVAIOModel]):
+    def select(self, *selection) -> AIOModelSelect[TVAIOModel]:
+        return AIOModelSelect(self, selection)
+
+
 class AIOModel(Model, metaclass=AIOModelBase):
     if TYPE_CHECKING:
         _manager: Manager
         _meta: Metadata
 
         DoesNotExist: Type[Exception]
 
@@ -242,14 +247,18 @@
 
         return n
 
     # Queryset methods
     # ----------------
 
     @classmethod
+    def alias(cls: Type[TVAIOModel], alias: Optional[str] = None) -> AIOModelAlias[TVAIOModel]:
+        return AIOModelAlias(cls, alias)
+
+    @classmethod
     def select(
         cls: Type[TVAIOModel], *select: Union[Type[Model], ColumnBase, Table, ModelAlias]
     ) -> AIOModelSelect[TVAIOModel]:
         return AIOModelSelect(
             cls,
             select or cls._meta.sorted_fields,
             is_default=not select,
```

### Comparing `peewee_aio-1.5.6/pyproject.toml` & `peewee_aio-1.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-aio"
-version = "1.5.6"
+version = "1.5.7"
 description = "Async support for Peewee ORM"
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/klen/peewee-aio"
 repository = "https://github.com/klen/peewee-aio"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["peewee", "asyncio", "trio", "orm"]
```

### Comparing `peewee_aio-1.5.6/PKG-INFO` & `peewee_aio-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-aio
-Version: 1.5.6
+Version: 1.5.7
 Summary: Async support for Peewee ORM
 Home-page: https://github.com/klen/peewee-aio
 License: MIT
 Keywords: peewee,asyncio,trio,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```


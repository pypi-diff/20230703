# Comparing `tmp/sqlalchemy_mock-1.0.5.tar.gz` & `tmp/sqlalchemy_mock-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_mock-1.0.5.tar", max compression
+gzip compressed data, was "sqlalchemy_mock-1.0.6.tar", max compression
```

## Comparing `sqlalchemy_mock-1.0.5.tar` & `sqlalchemy_mock-1.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.5/README.md
--rw-r--r--   0        0        0      448 2023-06-19 08:56:10.306028 sqlalchemy_mock-1.0.5/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-13 08:13:20.212930 sqlalchemy_mock-1.0.5/sqlalchemy_mock/__init__.py
--rw-r--r--   0        0        0      183 2023-06-13 08:13:20.213067 sqlalchemy_mock-1.0.5/sqlalchemy_mock/async_session.py
--rw-r--r--   0        0        0     6433 2023-06-19 08:55:36.792688 sqlalchemy_mock-1.0.5/sqlalchemy_mock/execute.py
--rw-r--r--   0        0        0     1427 2023-06-13 08:13:20.213390 sqlalchemy_mock-1.0.5/sqlalchemy_mock/query.py
--rw-r--r--   0        0        0     3369 2023-06-19 08:55:36.792865 sqlalchemy_mock-1.0.5/sqlalchemy_mock/session.py
--rw-r--r--   0        0        0     4575 2023-06-15 17:23:23.760224 sqlalchemy_mock-1.0.5/sqlalchemy_mock/utils.py
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.6/README.md
+-rw-r--r--   0        0        0      448 2023-07-03 19:55:22.578743 sqlalchemy_mock-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-13 08:13:20.212930 sqlalchemy_mock-1.0.6/sqlalchemy_mock/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-13 08:13:20.213067 sqlalchemy_mock-1.0.6/sqlalchemy_mock/async_session.py
+-rw-r--r--   0        0        0     6433 2023-06-19 08:55:36.792688 sqlalchemy_mock-1.0.6/sqlalchemy_mock/execute.py
+-rw-r--r--   0        0        0     1427 2023-06-13 08:13:20.213390 sqlalchemy_mock-1.0.6/sqlalchemy_mock/query.py
+-rw-r--r--   0        0        0     3508 2023-07-03 19:53:53.223210 sqlalchemy_mock-1.0.6/sqlalchemy_mock/session.py
+-rw-r--r--   0        0        0     4625 2023-07-03 19:53:53.224051 sqlalchemy_mock-1.0.6/sqlalchemy_mock/utils.py
+-rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.6/PKG-INFO
```

### Comparing `sqlalchemy_mock-1.0.5/README.md` & `sqlalchemy_mock-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.5/sqlalchemy_mock/execute.py` & `sqlalchemy_mock-1.0.6/sqlalchemy_mock/execute.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.5/sqlalchemy_mock/query.py` & `sqlalchemy_mock-1.0.6/sqlalchemy_mock/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.5/sqlalchemy_mock/session.py` & `sqlalchemy_mock-1.0.6/sqlalchemy_mock/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,18 @@
         label_columns = self.get_label_columns(record.__class__)
         record = self.process_sql_columns(record, label_columns)
         return record
 
     def mock_session(self):
         return mock_sessions_methods(self)
 
+    def bulk_insert_mappings(self, table, values):
+        records = [table(**record) for record in values]
+        self.add_all(records)
+
     def get_records_by_instance(self, instance: object):
         return self.__storage.get(str(instance), [])
 
     def execute(self, expresion: object, *args, **kwargs):
         if not getattr(expresion, "element", None) is None:
             expresion = expresion.element
```

### Comparing `sqlalchemy_mock-1.0.5/sqlalchemy_mock/utils.py` & `sqlalchemy_mock-1.0.6/sqlalchemy_mock/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,23 +29,23 @@
             value = column.default.arg
             if isinstance(column.default.arg, FunctionType):
                 value = functions.get(column.default.arg.__name__, value)()
             setattr(record, column.name, value)
 
 
 def mock_sessions_methods(session: object):
-    db_mock_methods = {method: unittest.mock.MagicMock(side_effect=getattr(session, method)) for method in ("query", "add", "add_all", "commit", "refresh", "execute")}
+    db_mock_methods = {method: unittest.mock.MagicMock(side_effect=getattr(session, method)) for method in ("query", "add", "add_all", "commit", "refresh", "execute", "bulk_insert_mappings")}
     return unittest.mock.patch.multiple(sqlalchemy.orm.Session, **db_mock_methods)
 
 
 def compare_record_with_filter(record: object, filter: object):
     def _base_filter_handler(record: object, filter: object):
         field = getattr(record, filter.left.name)
 
-        if isinstance(field, UUID):
+        if isinstance(field, UUID) or isinstance(field, int):
             field = str(field)
         elif not isinstance(field, str) and not isinstance(field, bool) and not field is None:
             field = field.value
 
         value = filter.right.value
         if not isinstance(value, str) and not isinstance(value, bool) and not value is None:
             value = str(value)
```

### Comparing `sqlalchemy_mock-1.0.5/PKG-INFO` & `sqlalchemy_mock-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-mock
-Version: 1.0.5
+Version: 1.0.6
 Summary: The package for working with SQLAlchemy in unit tests
 Author: ivanostapiuk
 Author-email: ost.ivan13@gmail.com
 Requires-Python: >=3.0,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```


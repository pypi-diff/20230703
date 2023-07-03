# Comparing `tmp/sqlalchemy-timescaledb-0.4.tar.gz` & `tmp/sqlalchemy-timescaledb-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-timescaledb-0.4.tar", last modified: Mon Feb 20 23:24:31 2023, max compression
+gzip compressed data, was "sqlalchemy-timescaledb-0.4.1.tar", last modified: Mon Jul  3 11:12:05 2023, max compression
```

## Comparing `sqlalchemy-timescaledb-0.4.tar` & `sqlalchemy-timescaledb-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 a-kletsko  (1000) a-kletsko  (1000)        0 2023-02-20 23:24:31.867023 sqlalchemy-timescaledb-0.4/
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     1074 2023-02-07 08:51:14.000000 sqlalchemy-timescaledb-0.4/LICENSE
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     2223 2023-02-20 23:24:31.867023 sqlalchemy-timescaledb-0.4/PKG-INFO
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     1895 2023-02-17 16:48:12.000000 sqlalchemy-timescaledb-0.4/README.md
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      975 2023-02-20 23:22:01.000000 sqlalchemy-timescaledb-0.4/pyproject.toml
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)       38 2023-02-20 23:24:31.867023 sqlalchemy-timescaledb-0.4/setup.cfg
-drwxrwxr-x   0 a-kletsko  (1000) a-kletsko  (1000)        0 2023-02-20 23:24:31.863023 sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb/
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      392 2023-02-20 23:21:55.000000 sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb/__init__.py
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     1725 2023-02-20 23:22:01.000000 sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb/dialect.py
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      215 2023-02-17 16:48:12.000000 sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb/functions.py
-drwxrwxr-x   0 a-kletsko  (1000) a-kletsko  (1000)        0 2023-02-20 23:24:31.867023 sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb.egg-info/
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     2223 2023-02-20 23:24:31.000000 sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb.egg-info/PKG-INFO
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      486 2023-02-20 23:24:31.000000 sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb.egg-info/SOURCES.txt
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)        1 2023-02-20 23:24:31.000000 sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb.egg-info/dependency_links.txt
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      254 2023-02-20 23:24:31.000000 sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb.egg-info/entry_points.txt
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      183 2023-02-20 23:24:31.000000 sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb.egg-info/requires.txt
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)       23 2023-02-20 23:24:31.000000 sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb.egg-info/top_level.txt
-drwxrwxr-x   0 a-kletsko  (1000) a-kletsko  (1000)        0 2023-02-20 23:24:31.867023 sqlalchemy-timescaledb-0.4/tests/
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      949 2023-02-20 23:22:01.000000 sqlalchemy-timescaledb-0.4/tests/test_alembic.py
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     2736 2023-02-20 23:22:01.000000 sqlalchemy-timescaledb-0.4/tests/test_functions.py
--rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      241 2023-02-20 22:49:51.000000 sqlalchemy-timescaledb-0.4/tests/test_hypertable.py
+drwxrwxr-x   0 a-kletsko  (1000) a-kletsko  (1000)        0 2023-07-03 11:12:05.066748 sqlalchemy-timescaledb-0.4.1/
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     1074 2023-02-07 08:51:14.000000 sqlalchemy-timescaledb-0.4.1/LICENSE
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     2834 2023-07-03 11:12:05.066748 sqlalchemy-timescaledb-0.4.1/PKG-INFO
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     2504 2023-07-03 11:07:06.000000 sqlalchemy-timescaledb-0.4.1/README.md
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      977 2023-07-03 11:11:10.000000 sqlalchemy-timescaledb-0.4.1/pyproject.toml
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)       38 2023-07-03 11:12:05.066748 sqlalchemy-timescaledb-0.4.1/setup.cfg
+drwxrwxr-x   0 a-kletsko  (1000) a-kletsko  (1000)        0 2023-07-03 11:12:05.066748 sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb/
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      392 2023-02-20 23:21:55.000000 sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb/__init__.py
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     2161 2023-07-03 11:07:06.000000 sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb/dialect.py
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      215 2023-02-17 16:48:12.000000 sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb/functions.py
+drwxrwxr-x   0 a-kletsko  (1000) a-kletsko  (1000)        0 2023-07-03 11:12:05.066748 sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb.egg-info/
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     2834 2023-07-03 11:12:05.000000 sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb.egg-info/PKG-INFO
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      513 2023-07-03 11:12:05.000000 sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb.egg-info/SOURCES.txt
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)        1 2023-07-03 11:12:05.000000 sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb.egg-info/dependency_links.txt
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      254 2023-07-03 11:12:05.000000 sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb.egg-info/entry_points.txt
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      183 2023-07-03 11:12:05.000000 sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb.egg-info/requires.txt
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)       23 2023-07-03 11:12:05.000000 sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb.egg-info/top_level.txt
+drwxrwxr-x   0 a-kletsko  (1000) a-kletsko  (1000)        0 2023-07-03 11:12:05.066748 sqlalchemy-timescaledb-0.4.1/tests/
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      949 2023-02-20 23:22:01.000000 sqlalchemy-timescaledb-0.4.1/tests/test_alembic.py
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     1312 2023-07-03 11:07:06.000000 sqlalchemy-timescaledb-0.4.1/tests/test_ddl_compiler.py
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)     2736 2023-02-20 23:22:01.000000 sqlalchemy-timescaledb-0.4.1/tests/test_functions.py
+-rw-rw-r--   0 a-kletsko  (1000) a-kletsko  (1000)      241 2023-02-20 22:49:51.000000 sqlalchemy-timescaledb-0.4.1/tests/test_hypertable.py
```

### Comparing `sqlalchemy-timescaledb-0.4/LICENSE` & `sqlalchemy-timescaledb-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-timescaledb-0.4/PKG-INFO` & `sqlalchemy-timescaledb-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-timescaledb
-Version: 0.4
+Version: 0.4.1
 Summary: A SQLAlchemy dialect for TimescaleDB
 Author-email: Andrei Kliatsko <andrey.daraschenka@gmail.com>
 Project-URL: Homepage, https://github.com/dorosch/sqlalchemy-timescaledb
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -45,31 +45,60 @@
         'time_column_name': 'timestamp'
     }
 )
 
 metadata.create_all(engine)
 ```
 
+Or using `declarative_base` style:
+
+```Python
+import datetime
+
+from sqlalchemy.orm import declarative_base
+from sqlalchemy import Column, Float, String, DateTime
+
+Base = declarative_base()
+
+class Metric(Base):
+    __table_args__ = ({
+        'timescaledb_hypertable': {
+            'time_column_name': 'timestamp'
+        }
+    })
+
+    name = Column(String)
+    value = Column(Float)
+    timestamp = Column(
+        DateTime(), default=datetime.datetime.now, primary_key=True
+    )
+```
+
+## Parameters
+
+* [chunk_time_interval](6)
+
 ## Functions
 
 Timescaledb functions implemented:
 
-### [first(value, time)][6]
+### [first(value, time)][7]
 
 ```Python
 func.first(Metric.value, Metric.timestamp)
 ```
 
-### [last(value, time)][7]
+### [last(value, time)][8]
 
 ```Python
 func.last(Metric.value, Metric.timestamp)
 ```
 
 
 [1]: https://badge.fury.io/py/sqlalchemy-timescaledb
 [2]: https://github.com/dorosch/sqlalchemy-timescaledb/actions/workflows/tests.yml
 [3]: https://codecov.io/gh/dorosch/sqlalchemy-timescaledb
 [4]: https://pepy.tech/project/sqlalchemy-timescaledb
 [5]: https://docs.timescale.com/api/latest/hypertable/create_hypertable/#optional-arguments
-[6]: https://docs.timescale.com/api/latest/hyperfunctions/first/
-[7]: https://docs.timescale.com/api/latest/hyperfunctions/last/
+[6]: https://docs.timescale.com/api/latest/hypertable/set_chunk_time_interval/
+[7]: https://docs.timescale.com/api/latest/hyperfunctions/first/
+[8]: https://docs.timescale.com/api/latest/hyperfunctions/last/
```

### Comparing `sqlalchemy-timescaledb-0.4/README.md` & `sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: sqlalchemy-timescaledb
+Version: 0.4.1
+Summary: A SQLAlchemy dialect for TimescaleDB
+Author-email: Andrei Kliatsko <andrey.daraschenka@gmail.com>
+Project-URL: Homepage, https://github.com/dorosch/sqlalchemy-timescaledb
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # SQLAlchemy TimescaleDB
 
 [![PyPI version](https://badge.fury.io/py/sqlalchemy-timescaledb.svg)][1]
 [![Tests](https://github.com/dorosch/sqlalchemy-timescaledb/actions/workflows/tests.yml/badge.svg)][2]
 [![codecov](https://codecov.io/gh/dorosch/sqlalchemy-timescaledb/branch/develop/graph/badge.svg?token=Gzh7KpADjZ)][3]
 [![Downloads](https://pepy.tech/badge/sqlalchemy-timescaledb)][4]
 
@@ -35,31 +45,60 @@
         'time_column_name': 'timestamp'
     }
 )
 
 metadata.create_all(engine)
 ```
 
+Or using `declarative_base` style:
+
+```Python
+import datetime
+
+from sqlalchemy.orm import declarative_base
+from sqlalchemy import Column, Float, String, DateTime
+
+Base = declarative_base()
+
+class Metric(Base):
+    __table_args__ = ({
+        'timescaledb_hypertable': {
+            'time_column_name': 'timestamp'
+        }
+    })
+
+    name = Column(String)
+    value = Column(Float)
+    timestamp = Column(
+        DateTime(), default=datetime.datetime.now, primary_key=True
+    )
+```
+
+## Parameters
+
+* [chunk_time_interval](6)
+
 ## Functions
 
 Timescaledb functions implemented:
 
-### [first(value, time)][6]
+### [first(value, time)][7]
 
 ```Python
 func.first(Metric.value, Metric.timestamp)
 ```
 
-### [last(value, time)][7]
+### [last(value, time)][8]
 
 ```Python
 func.last(Metric.value, Metric.timestamp)
 ```
 
 
 [1]: https://badge.fury.io/py/sqlalchemy-timescaledb
 [2]: https://github.com/dorosch/sqlalchemy-timescaledb/actions/workflows/tests.yml
 [3]: https://codecov.io/gh/dorosch/sqlalchemy-timescaledb
 [4]: https://pepy.tech/project/sqlalchemy-timescaledb
 [5]: https://docs.timescale.com/api/latest/hypertable/create_hypertable/#optional-arguments
-[6]: https://docs.timescale.com/api/latest/hyperfunctions/first/
-[7]: https://docs.timescale.com/api/latest/hyperfunctions/last/
+[6]: https://docs.timescale.com/api/latest/hypertable/set_chunk_time_interval/
+[7]: https://docs.timescale.com/api/latest/hyperfunctions/first/
+[8]: https://docs.timescale.com/api/latest/hyperfunctions/last/
```

### Comparing `sqlalchemy-timescaledb-0.4/pyproject.toml` & `sqlalchemy-timescaledb-0.4.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sqlalchemy-timescaledb"
-version = "0.4"
+version = "0.4.1"
 authors = [
   { name="Andrei Kliatsko", email="andrey.daraschenka@gmail.com" },
 ]
 description = "A SQLAlchemy dialect for TimescaleDB"
 readme = "README.md"
 dependencies = [
     "sqlalchemy>=1.3"
```

### Comparing `sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb/dialect.py` & `sqlalchemy-timescaledb-0.4.1/sqlalchemy_timescaledb/dialect.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,19 +29,29 @@
                 )
             )
 
         return super().post_create_table(table)
 
     @staticmethod
     def ddl_hypertable(table_name, hypertable):
+        time_column_name = hypertable['time_column_name']
+        chunk_time_interval = hypertable.get('chunk_time_interval', '7 days')
+
+        if isinstance(chunk_time_interval, str):
+            if chunk_time_interval.isdigit():
+                chunk_time_interval = int(chunk_time_interval)
+            else:
+                chunk_time_interval = f"INTERVAL '{chunk_time_interval}'"
+
         return DDL(
             f"""
             SELECT create_hypertable(
                 '{table_name}',
-                '{hypertable['time_column_name']}',
+                '{time_column_name}',
+                chunk_time_interval => {chunk_time_interval},
                 if_not_exists => TRUE
             );
             """
         )
 
 
 class TimescaledbDialect:
```

### Comparing `sqlalchemy-timescaledb-0.4/sqlalchemy_timescaledb.egg-info/PKG-INFO` & `sqlalchemy-timescaledb-0.4.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: sqlalchemy-timescaledb
-Version: 0.4
-Summary: A SQLAlchemy dialect for TimescaleDB
-Author-email: Andrei Kliatsko <andrey.daraschenka@gmail.com>
-Project-URL: Homepage, https://github.com/dorosch/sqlalchemy-timescaledb
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # SQLAlchemy TimescaleDB
 
 [![PyPI version](https://badge.fury.io/py/sqlalchemy-timescaledb.svg)][1]
 [![Tests](https://github.com/dorosch/sqlalchemy-timescaledb/actions/workflows/tests.yml/badge.svg)][2]
 [![codecov](https://codecov.io/gh/dorosch/sqlalchemy-timescaledb/branch/develop/graph/badge.svg?token=Gzh7KpADjZ)][3]
 [![Downloads](https://pepy.tech/badge/sqlalchemy-timescaledb)][4]
 
@@ -45,31 +35,60 @@
         'time_column_name': 'timestamp'
     }
 )
 
 metadata.create_all(engine)
 ```
 
+Or using `declarative_base` style:
+
+```Python
+import datetime
+
+from sqlalchemy.orm import declarative_base
+from sqlalchemy import Column, Float, String, DateTime
+
+Base = declarative_base()
+
+class Metric(Base):
+    __table_args__ = ({
+        'timescaledb_hypertable': {
+            'time_column_name': 'timestamp'
+        }
+    })
+
+    name = Column(String)
+    value = Column(Float)
+    timestamp = Column(
+        DateTime(), default=datetime.datetime.now, primary_key=True
+    )
+```
+
+## Parameters
+
+* [chunk_time_interval](6)
+
 ## Functions
 
 Timescaledb functions implemented:
 
-### [first(value, time)][6]
+### [first(value, time)][7]
 
 ```Python
 func.first(Metric.value, Metric.timestamp)
 ```
 
-### [last(value, time)][7]
+### [last(value, time)][8]
 
 ```Python
 func.last(Metric.value, Metric.timestamp)
 ```
 
 
 [1]: https://badge.fury.io/py/sqlalchemy-timescaledb
 [2]: https://github.com/dorosch/sqlalchemy-timescaledb/actions/workflows/tests.yml
 [3]: https://codecov.io/gh/dorosch/sqlalchemy-timescaledb
 [4]: https://pepy.tech/project/sqlalchemy-timescaledb
 [5]: https://docs.timescale.com/api/latest/hypertable/create_hypertable/#optional-arguments
-[6]: https://docs.timescale.com/api/latest/hyperfunctions/first/
-[7]: https://docs.timescale.com/api/latest/hyperfunctions/last/
+[6]: https://docs.timescale.com/api/latest/hypertable/set_chunk_time_interval/
+[7]: https://docs.timescale.com/api/latest/hyperfunctions/first/
+[8]: https://docs.timescale.com/api/latest/hyperfunctions/last/
```

### Comparing `sqlalchemy-timescaledb-0.4/tests/test_alembic.py` & `sqlalchemy-timescaledb-0.4.1/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-timescaledb-0.4/tests/test_functions.py` & `sqlalchemy-timescaledb-0.4.1/tests/test_functions.py`

 * *Files identical despite different names*


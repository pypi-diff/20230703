# Comparing `tmp/mysqlx-1.3.2.tar.gz` & `tmp/mysqlx-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.3.2.tar", last modified: Sun Jul  2 08:03:57 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.3.3.tar", last modified: Sun Jul  2 22:54:55 2023, max compression
```

## Comparing `mysqlx-1.3.2.tar` & `mysqlx-1.3.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 08:03:56.000000 mysqlx-1.3.2/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx/
--rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.3.2/mysqlx/coder.py
--rw-rw-rw-   0        0        0     1644 2023-06-26 14:04:23.000000 mysqlx-1.3.2/mysqlx/coder.tpl
--rw-rw-rw-   0        0        0    19388 2023-07-01 16:17:50.000000 mysqlx-1.3.2/mysqlx/db.py
--rw-rw-rw-   0        0        0    13200 2023-07-02 03:56:40.000000 mysqlx-1.3.2/mysqlx/dbx.py
--rw-rw-rw-   0        0        0    36870 2023-07-01 16:20:03.000000 mysqlx-1.3.2/mysqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.3.2/mysqlx/snowflake.py
--rw-rw-rw-   0        0        0     3596 2023-07-02 06:28:56.000000 mysqlx-1.3.2/mysqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     7811 2023-06-30 06:21:34.000000 mysqlx-1.3.2/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.2/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.3.2/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4247 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      589 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4247 2023-07-02 08:03:56.000000 mysqlx-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3712 2023-07-02 07:35:05.000000 mysqlx-1.3.2/README.md
--rw-rw-rw-   0        0        0     4185 2023-06-20 09:05:43.000000 mysqlx-1.3.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-02 08:03:56.000000 mysqlx-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1233 2023-07-02 08:03:49.000000 mysqlx-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:03:56.000000 mysqlx-1.3.2/test/
--rw-rw-rw-   0        0        0      216 2023-06-25 13:41:37.000000 mysqlx-1.3.2/test/all_unit_test.py
--rw-rw-rw-   0        0        0      312 2023-06-19 03:27:12.000000 mysqlx-1.3.2/test/coder_test.py
--rw-rw-rw-   0        0        0     2988 2023-07-02 06:29:16.000000 mysqlx-1.3.2/test/dbx_test.py
--rw-rw-rw-   0        0        0     5067 2023-06-27 15:48:31.000000 mysqlx-1.3.2/test/db_test.py
--rw-rw-rw-   0        0        0      770 2023-07-02 04:45:13.000000 mysqlx-1.3.2/test/mapper_test.py
--rw-rw-rw-   0        0        0     5202 2023-07-01 16:10:46.000000 mysqlx-1.3.2/test/models.py
--rw-rw-rw-   0        0        0     5648 2023-07-01 16:10:25.000000 mysqlx-1.3.2/test/orm_test.py
--rw-rw-rw-   0        0        0      301 2023-06-26 13:41:30.000000 mysqlx-1.3.2/test/snowflake_test.py
--rw-rw-rw-   0        0        0      381 2023-06-21 05:03:37.000000 mysqlx-1.3.2/test/time_test.py
--rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.3.2/test/unit_test.py
--rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.3.2/test/user_mapper.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 22:54:55.000000 mysqlx-1.3.3/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-02 22:54:55.000000 mysqlx-1.3.3/mysqlx/
+-rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.3.3/mysqlx/coder.py
+-rw-rw-rw-   0        0        0     1644 2023-06-26 14:04:23.000000 mysqlx-1.3.3/mysqlx/coder.tpl
+-rw-rw-rw-   0        0        0    20093 2023-07-02 22:53:10.000000 mysqlx-1.3.3/mysqlx/db.py
+-rw-rw-rw-   0        0        0    13200 2023-07-02 03:56:40.000000 mysqlx-1.3.3/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0    36870 2023-07-01 16:20:03.000000 mysqlx-1.3.3/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.3.3/mysqlx/snowflake.py
+-rw-rw-rw-   0        0        0     3773 2023-07-02 22:43:31.000000 mysqlx-1.3.3/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     7811 2023-06-30 06:21:34.000000 mysqlx-1.3.3/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.3/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 22:54:55.000000 mysqlx-1.3.3/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-02 22:54:55.000000 mysqlx-1.3.3/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.3.3/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4248 2023-07-02 22:54:55.000000 mysqlx-1.3.3/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-07-02 22:54:55.000000 mysqlx-1.3.3/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      589 2023-07-02 22:54:55.000000 mysqlx-1.3.3/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-07-02 22:54:55.000000 mysqlx-1.3.3/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4248 2023-07-02 22:54:55.000000 mysqlx-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3449 2023-07-02 07:59:31.000000 mysqlx-1.3.3/README.md
+-rw-rw-rw-   0        0        0     4185 2023-06-20 09:05:43.000000 mysqlx-1.3.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-02 22:54:55.000000 mysqlx-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2023-07-02 22:54:31.000000 mysqlx-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 22:54:55.000000 mysqlx-1.3.3/test/
+-rw-rw-rw-   0        0        0      216 2023-06-25 13:41:37.000000 mysqlx-1.3.3/test/all_unit_test.py
+-rw-rw-rw-   0        0        0      312 2023-06-19 03:27:12.000000 mysqlx-1.3.3/test/coder_test.py
+-rw-rw-rw-   0        0        0     2988 2023-07-02 06:29:16.000000 mysqlx-1.3.3/test/dbx_test.py
+-rw-rw-rw-   0        0        0     5067 2023-06-27 15:48:31.000000 mysqlx-1.3.3/test/db_test.py
+-rw-rw-rw-   0        0        0      787 2023-07-02 22:53:26.000000 mysqlx-1.3.3/test/mapper_test.py
+-rw-rw-rw-   0        0        0     5202 2023-07-01 16:10:46.000000 mysqlx-1.3.3/test/models.py
+-rw-rw-rw-   0        0        0     5648 2023-07-01 16:10:25.000000 mysqlx-1.3.3/test/orm_test.py
+-rw-rw-rw-   0        0        0      301 2023-06-26 13:41:30.000000 mysqlx-1.3.3/test/snowflake_test.py
+-rw-rw-rw-   0        0        0      381 2023-06-21 05:03:37.000000 mysqlx-1.3.3/test/time_test.py
+-rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.3.3/test/unit_test.py
+-rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.3.3/test/user_mapper.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.3/test/__init__.py
```

### Comparing `mysqlx-1.3.2/LICENSE` & `mysqlx-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.2/mysqlx/coder.py` & `mysqlx-1.3.3/mysqlx/coder.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.2/mysqlx/coder.tpl` & `mysqlx-1.3.3/mysqlx/coder.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.2/mysqlx/db.py` & `mysqlx-1.3.3/mysqlx/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,24 @@
         from mysql.connector import connect
         use_mysql_connector = True
     except ImportError:
         from pymysql import connect
 
     global _DB_CTX
     global _SHOW_SQL
+
+    if 'debug' in kwargs:
+        if kwargs['debug']:
+            logging.basicConfig(level=logging.DEBUG, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+        else:
+            logging.basicConfig(level=logging.INFO, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+        del kwargs['debug']
+    else:
+        logging.basicConfig(level=logging.INFO, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+
     is_pool = use_mysql_connector and pool_size >= 1
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
         _SHOW_SQL = show_sql
         if _MAPPER_PATH in kwargs:
             from .dbx import load_mapper
@@ -116,27 +126,37 @@
     return: Effect rowcount
     """
     logging.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', kwargs: %s" % ('insert', table, kwargs))
     sql, args = _insert_sql_args(table.strip(), **kwargs)
     return do_execute(sql, *args)
 
 
-@with_connection
 def save(table: str, **kwargs):
     """
     Execute insert SQL, return primary key.
-    :param table: table name
-    :param kwargs: name='张三', age=20}
+    :param table: table
+    :param kwargs: name='张三', age=20
     :return: Primary key
     """
     logging.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', kwargs: %s" % ('save', table, kwargs))
+    sql, args = _insert_sql_args(table.strip(), **kwargs)
+    return do_save(sql, *args)
+
+
+@with_connection
+def do_save(sql: str, *args):
+    """
+    Execute insert SQL, return primary key.
+    :param sql: table
+    :param args:
+    :return: Primary key
+    """
     global _DB_CTX
     cursor = None
-    sql, args = _insert_sql_args(table.strip(), **kwargs)
-    sql = _before_execute('save', sql, *args)
+    sql = _before_execute('do_save', sql, *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         cursor.execute(_PK_SQL)
         result = cursor.fetchone()
         try_commit(_DB_CTX)
         return result[0]
```

### Comparing `mysqlx-1.3.2/mysqlx/dbx.py` & `mysqlx-1.3.3/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.2/mysqlx/orm.py` & `mysqlx-1.3.3/mysqlx/orm.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.2/mysqlx/snowflake.py` & `mysqlx-1.3.3/mysqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.2/mysqlx/sql_mapper.py` & `mysqlx-1.3.3/mysqlx/sql_mapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,72 @@
 import os
 import logging
 import functools
 from .support import SqlAction, get_named_sql_args, simple_sql
 from .dbx import get_sql_model, do_get_sql, build_sql_id
-from .db import do_get, do_query, do_query_one, do_execute, do_batch_execute, do_select, do_select_one, batch_execute
+from .db import do_get, do_query, do_query_one, do_execute, do_batch_execute, do_select, do_select_one, batch_execute, do_save
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
-def mapper(namespace: str = None, sql_id: str = None, batch: bool = False):
+def mapper(namespace: str = None, sql_id: str = None, batch=False, return_pk=False):
     def _decorator(func):
         @functools.wraps(func)
         def _wrapper(*args, **kwargs):
             param_names = func.__code__.co_varnames
             full_sql_id, func_name = _before(func, namespace, sql_id, *args, **kwargs)
             sql_model = get_sql_model(full_sql_id)
-            exec_func = _get_exec_func(func, sql_model.action, batch)
+            exec_func = _get_exec_func(func, sql_model.action, batch, return_pk)
             if not batch:
                 use_sql, args = do_get_sql(sql_model, batch, param_names, *args, **kwargs)
             else:
                 if kwargs:
                     logging.warning("Batch exec sql better use like '{}(args)' or '{}(*args)' then '{}(args=args)'".format(func_name, func_name, func_name))
                     args = list(kwargs.values())[0]
                 use_sql, _ = do_get_sql(sql_model, batch, param_names, *args)
             return exec_func(use_sql, *args)
 
         return _wrapper
     return _decorator
 
 
-def sql(value: str, batch: bool = False):
+def sql(value: str, batch=False, return_pk=False):
     def _decorator(func):
         @functools.wraps(func)
         def _wrapper(*args, **kwargs):
             use_sql = value
             low_sql = value.lower()
             if any([action in low_sql for action in _UPDATE_ACTIONS]):
                 if batch:
                     if kwargs:
                         args = list(kwargs.values())[0]
                     return batch_execute(use_sql, *args)
                 if kwargs:
                     use_sql, args = get_named_sql_args(**kwargs)
+                if return_pk:
+                    return do_save(use_sql, *args)
                 return do_execute(use_sql, *args)
             elif SqlAction.SELECT.value in low_sql:
                 select_func = _get_select_func(func)
                 use_sql, args = simple_sql(use_sql, *args, **kwargs)
                 return select_func(use_sql, *args)
             else:
                 return ValueError("Invalid sql: {}.".format(sql))
 
         return _wrapper
     return _decorator
 
 
-def _get_exec_func(func, action, batch):
+def _get_exec_func(func, action, batch, return_pk):
     if action == SqlAction.SELECT.value:
         return _get_select_func(func)
     elif batch:
         return do_batch_execute
+    elif return_pk:
+        return do_save
     else:
         return do_execute
 
 
 def _get_select_func(func):
     names = func.__code__.co_names
     is_list = 'list' in names or 'List' in names
```

### Comparing `mysqlx-1.3.2/mysqlx/support.py` & `mysqlx-1.3.3/mysqlx/support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.2/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.3.3/mysqlx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.3.2
-Summary: MySqlx is a simple python sql executor for MySQL like iBatis.
+Version: 1.3.3
+Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
```

### Comparing `mysqlx-1.3.2/mysqlx.egg-info/SOURCES.txt` & `mysqlx-1.3.3/mysqlx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.2/PKG-INFO` & `mysqlx-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.3.2
-Summary: MySqlx is a simple python sql executor for MySQL like iBatis.
+Version: 1.3.3
+Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
```

### Comparing `mysqlx-1.3.2/README.md` & `mysqlx-1.3.3/test/db_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,87 @@
-##### Install
-```
-pip install mysqlx
-```
-##### Usage Sample
-```
+import logging
+from mysqlx import db
+from config import DB_CONF
+
+create_table_sql = '''
 CREATE TABLE `user` (
-  `id` bigint NOT NULL AUTO_INCREMENT,
+  `id` bigint unsigned NOT NULL AUTO_INCREMENT,
   `name` varchar(45) NOT NULL,
-  `age` int NOT NULL,
+  `age` int unsigned NOT NULL,
   `birth_date` date DEFAULT NULL,
-  `sex` tinyint DEFAULT NULL,
+  `sex` tinyint unsigned DEFAULT NULL,
+  `grade` float DEFAULT NULL,
+  `point` double DEFAULT NULL,
+  `money` decimal(8,4) DEFAULT NULL,
+  `create_by` bigint DEFAULT NULL,
+  `create_time` datetime DEFAULT CURRENT_TIMESTAMP,
+  `update_by` bigint DEFAULT NULL,
+  `update_time` datetime DEFAULT NULL,
+  `del_flag` tinyint NOT NULL DEFAULT '0',
   PRIMARY KEY (`id`)
 ) ENGINE=InnoDB AUTO_INCREMENT=62 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci
+'''
 
 
-----------------------------------------------------------------------------------------
+def create_truncate_table(table):
+    cnt = db.do_get("SELECT count(1) FROM information_schema.TABLES WHERE table_schema=database() AND table_name=?", table)
+    if cnt == 0:
+        db.do_execute(create_table_sql)
+    else:
+        db.do_execute('truncate table %s' % table)
 
-from mysqlx import db
 
-db_conf = {
-    'host': '127.0.0.1',
-    'port': 3306, 
-    'user': 'root', 
-    'password': 'xxx', 
-    'database': 'test',
-    'pool_size': 5,
-    'show_sql': True
-}
+def drop_table():
+    db.execute('DROP TABLE IF EXISTS user')
+
+
+@db.with_transaction
+def test_transaction(rollback: bool = False):
+    db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    assert db.get('select count(1) from user limit 1') == 4, 'transaction'
+    if rollback:
+        1 / 0
+    db.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+
+
+def test_transaction2(rollback: bool = False):
+    with db.transaction():
+        db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+        assert db.get('select count(1) from user') == 6, 'transaction2'
+        if rollback:
+            1 / 0
+        db.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+
+
+def full_test():
+    create_truncate_table('user')
+    #######################################################################################################
 
-if __name__ == '__main__':
-    db.init_db(**db_conf)
-    
-    # Return effect rowcount
     rowcount = db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-    assert rowcount == 1, '1 effect rowcount'
-    assert db.get('select count(1) from user') == 1, 'count is 1'
+    assert rowcount == 1, 'insert'
+    assert db.get('select count(1) from user') == 1, 'insert'
 
-    # Return primary key
     id2 = db.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-    assert db.get('select count(1) from user') == 2, 'count is 2'
+    assert id2 > 0, 'save'
+    assert db.get('select count(1) from user') == 2, 'save'
 
     db.execute('update user set name=? where id=?', '王五', id2)
     assert db.get('select name from user where id=?', id2) == '王五', 'execute'
 
     db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
     assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
 
     db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
     assert db.query_one('select name from user where id=:id', id=id2)['name'] == '赵六', 'execute'
 
     args = [
         ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56),
         ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56)
     ]
-    db.batch_execute('insert into user(name, age, birth_date, sex, grade, point, money) values(?,?,?,?,?,?,?)', args)
+    db.batch_execute('insert into user(name, age, birth_date, sex, grade, point, money) values(?,?,?,?,?,?,?)', *args)
     users = db.select('select id, del_flag from user')
     assert len(users) == 4, 'batch_execute'
     users = db.query('select id, del_flag from user')
     assert len(users) == 4, 'batch_execute'
 
     users = db.select('select id, del_flag from user where id=?', id2)
     assert len(users) == 1, 'select'
@@ -67,31 +91,42 @@
     users = db.select('select id, del_flag from user where id=:id', id=id2)
     assert len(users) == 1, 'select'
     users = db.query('select id, del_flag from user where id=:id', id=id2)
     assert len(users) == 1, 'select'
 
     db.execute('delete from user where id=? limit 1', id2)
     assert db.get('select count(1) from user') == 3, 'execute delete'
-```
-##### Transaction
-```
-@db.with_transaction
-def test_transaction():
-    db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-    db.insert('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+
+    try:
+        test_transaction(rollback=True)
+    except Exception:
+        print('Rollback.')
+    assert db.get('select count(1) from user') == 3, 'transaction'
+
+    test_transaction(rollback=False)
+    assert db.get('select count(1) from user') == 5, 'transaction'
+
+    try:
+        test_transaction2(rollback=True)
+    except Exception:
+        print('Rollback.')
+    assert db.get('select count(1) from user') == 5, 'transaction2'
+
+    test_transaction2(rollback=False)
+    assert db.get('select count(1) from user') == 7, 'transaction2'
+
+
+if __name__ == '__main__':
+    logging.basicConfig(level=logging.DEBUG, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+    db.init_db(**DB_CONF, pool_size=2)
+    # drop_table()
+    full_test()
+
+
+    # for u in db.select('select * from user'):
+    #     print(u)
+    #
+    # for u in db.select_page('select * from user', 2, 3):
+    #     print(u)
+
 
 
-def test_transaction2():
-    with db.transaction():
-        db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-        db.insert('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-```
-##### Note: the functions return type
-```
-get: Return only one object, like count
-query_one: Return one row with dict
-select_one: Return one row with tuple
-find_by_id: Return one row with class instance object
-query: Return list of dict
-select: Return list of tuple
-find: Return list of class instance object
-```
```

### Comparing `mysqlx-1.3.2/README.rst` & `mysqlx-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.2/setup.py` & `mysqlx-1.3.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,22 +10,22 @@
         return fp.read()
 
 long_description = read("README_en.rst")
 
 setup(
     name='mysqlx',
     packages=find_packages(),
-    description="MySqlx is a simple python sql executor for MySQL like iBatis.",
+    description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.3.2',
+    version='1.3.3',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `mysqlx-1.3.2/test/dbx_test.py` & `mysqlx-1.3.3/test/dbx_test.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.2/test/mapper_test.py` & `mysqlx-1.3.3/test/mapper_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from mysqlx import db
 from test.mapper import user
 
 if __name__ == '__main__':
     from config import DB_CONF
-    import logging
-    logging.basicConfig(level=logging.DEBUG, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
-    db.init_db(**DB_CONF)
+    # import logging
+    # logging.basicConfig(level=logging.DEBUG, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+    db.init_db(**DB_CONF, debug=False)
     args = [
         ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56),
         ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56)
     ]
     user.batch_insert(args)
 
     print(user.select_name(4))
```

### Comparing `mysqlx-1.3.2/test/models.py` & `mysqlx-1.3.3/test/models.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.2/test/orm_test.py` & `mysqlx-1.3.3/test/orm_test.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.2/test/unit_test.py` & `mysqlx-1.3.3/test/unit_test.py`

 * *Files identical despite different names*


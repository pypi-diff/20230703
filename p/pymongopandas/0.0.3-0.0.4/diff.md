# Comparing `tmp/pymongopandas-0.0.3-py3-none-any.whl.zip` & `tmp/pymongopandas-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3655 bytes, number of entries: 7
--rw-r--r--  2.0 unx     3804 b- defN 23-Mar-09 14:54 DBClient/DBClient.py
+Zip file size: 3664 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     3824 b- defN 23-Jul-03 16:15 DBClient/DBClient.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-16 11:33 DBClient/__init__.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Mar-09 15:01 pymongopandas-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      627 b- defN 23-Mar-09 15:01 pymongopandas-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-09 15:01 pymongopandas-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Mar-09 15:01 pymongopandas-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      565 b- defN 23-Mar-09 15:01 pymongopandas-0.0.3.dist-info/RECORD
-7 files, 6170 bytes uncompressed, 2643 bytes compressed:  57.2%
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jul-03 16:20 pymongopandas-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-03 16:20 pymongopandas-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 16:20 pymongopandas-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-03 16:20 pymongopandas-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      565 b- defN 23-Jul-03 16:20 pymongopandas-0.0.4.dist-info/RECORD
+7 files, 6190 bytes uncompressed, 2652 bytes compressed:  57.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: DBClient/DBClient.py
 Comment: 
 
 Filename: DBClient/__init__.py
 Comment: 
 
-Filename: pymongopandas-0.0.3.dist-info/LICENSE
+Filename: pymongopandas-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: pymongopandas-0.0.3.dist-info/METADATA
+Filename: pymongopandas-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: pymongopandas-0.0.3.dist-info/WHEEL
+Filename: pymongopandas-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pymongopandas-0.0.3.dist-info/top_level.txt
+Filename: pymongopandas-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pymongopandas-0.0.3.dist-info/RECORD
+Filename: pymongopandas-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## DBClient/DBClient.py

```diff
@@ -26,16 +26,16 @@
 class DBClient:
     client: MongoClient
     db: Database
     collections: List[str]
     id_key: str
     progress_bar: bool
 
-    def __init__(self, connection_string: str, db_name: str, id_key: str = None, progress_bar=False):
-        self.client = MongoClient(connection_string)
+    def __init__(self, connection_string: str, db_name: str, id_key: str = None, progress_bar=False, **kwargs):
+        self.client = MongoClient(connection_string, **kwargs)
         self.db = self.get_db(db_name)
         self.collections = self.db.list_collection_names()
         self.id_key = id_key if id_key else '_id'
         self.progress_bar = progress_bar
 
     def get_db(self, db_name: str):
         return self.client[db_name]
```

## Comparing `pymongopandas-0.0.3.dist-info/LICENSE` & `pymongopandas-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pymongopandas-0.0.3.dist-info/METADATA` & `pymongopandas-0.0.4.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongopandas
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wraps pymongo to easily interact with pandas dataframes
 Home-page: https://github.com/JackFener/pymongo-pandas
 Author: Giacomo Fava
 Author-email: Giacomo Fava <giacomofava93@gmail.com>
 Project-URL: Homepage, https://github.com/JackFener/pymongo-pandas
 Project-URL: Bug Tracker, https://github.com/JackFener/pymongo-pandas/issues
 Classifier: Programming Language :: Python :: 3
```


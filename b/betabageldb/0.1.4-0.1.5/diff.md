# Comparing `tmp/betabageldb-0.1.4.tar.gz` & `tmp/betabageldb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betabageldb-0.1.4.tar", last modified: Mon Jul  3 11:06:13 2023, max compression
+gzip compressed data, was "betabageldb-0.1.5.tar", last modified: Mon Jul  3 13:23:20 2023, max compression
```

## Comparing `betabageldb-0.1.4.tar` & `betabageldb-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-03 11:06:13.213338 betabageldb-0.1.4/
--rw-r--r--   0 bidhan     (501) staff       (20)     5921 2023-07-01 11:14:26.000000 betabageldb-0.1.4/BagelDB.py
--rw-r--r--   0 bidhan     (501) staff       (20)       82 2023-06-27 19:31:31.000000 betabageldb-0.1.4/LICENSE.txt
--rw-r--r--   0 bidhan     (501) staff       (20)     4384 2023-07-03 11:06:13.213109 betabageldb-0.1.4/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)     3753 2023-07-01 11:28:45.000000 betabageldb-0.1.4/README.md
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-03 11:06:13.212734 betabageldb-0.1.4/betabageldb.egg-info/
--rw-r--r--   0 bidhan     (501) staff       (20)     4384 2023-07-03 11:06:13.000000 betabageldb-0.1.4/betabageldb.egg-info/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)      215 2023-07-03 11:06:13.000000 betabageldb-0.1.4/betabageldb.egg-info/SOURCES.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-03 11:06:13.000000 betabageldb-0.1.4/betabageldb.egg-info/dependency_links.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        9 2023-07-03 11:06:13.000000 betabageldb-0.1.4/betabageldb.egg-info/requires.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        8 2023-07-03 11:06:13.000000 betabageldb-0.1.4/betabageldb.egg-info/top_level.txt
--rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-03 11:06:13.213409 betabageldb-0.1.4/setup.cfg
--rw-r--r--   0 bidhan     (501) staff       (20)      795 2023-07-03 10:58:28.000000 betabageldb-0.1.4/setup.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-03 13:23:20.544093 betabageldb-0.1.5/
+-rw-r--r--   0 bidhan     (501) staff       (20)     6088 2023-07-03 13:19:31.000000 betabageldb-0.1.5/BagelDB.py
+-rw-r--r--   0 bidhan     (501) staff       (20)       82 2023-06-27 19:31:31.000000 betabageldb-0.1.5/LICENSE.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)     4384 2023-07-03 13:23:20.543886 betabageldb-0.1.5/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)     3753 2023-07-01 11:28:45.000000 betabageldb-0.1.5/README.md
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-03 13:23:20.543478 betabageldb-0.1.5/betabageldb.egg-info/
+-rw-r--r--   0 bidhan     (501) staff       (20)     4384 2023-07-03 13:23:20.000000 betabageldb-0.1.5/betabageldb.egg-info/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)      215 2023-07-03 13:23:20.000000 betabageldb-0.1.5/betabageldb.egg-info/SOURCES.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-03 13:23:20.000000 betabageldb-0.1.5/betabageldb.egg-info/dependency_links.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        9 2023-07-03 13:23:20.000000 betabageldb-0.1.5/betabageldb.egg-info/requires.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        8 2023-07-03 13:23:20.000000 betabageldb-0.1.5/betabageldb.egg-info/top_level.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-03 13:23:20.544137 betabageldb-0.1.5/setup.cfg
+-rw-r--r--   0 bidhan     (501) staff       (20)      795 2023-07-03 13:22:47.000000 betabageldb-0.1.5/setup.py
```

### Comparing `betabageldb-0.1.4/BagelDB.py` & `betabageldb-0.1.5/BagelDB.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,45 +79,50 @@
         if not isinstance(vectors, list):
             raise ValueError("Vectors must be an array")
 
         for vector in vectors:
             if not ('id' in vector and isinstance(vector['values'], list) and isinstance(vector['metadata'], dict)):
                 raise ValueError("Each vector must be an object with an 'id', 'values' array, and 'metadata' object")
 
+        headers = {'Content-Type': 'application/json'}
+
         data = {
             "index": self.index,
             "vectors": vectors
         }
 
         try:
-            response = requests.post(f'{self.baseURL}/v0/insert', data=json.dumps(data))
+            response = requests.post(f'{self.baseURL}/v0/insert', headers=headers, data=json.dumps(data))
             response.raise_for_status()
             return response.json()
         except requests.exceptions.RequestException as err:
             print(f'Request failed: {err}')
 
+
     def search(self, vector):
         """
         Method to search for a vector in the initialized index in BagelDB.
         
         :param vector: The vector for which the search is to be performed.
         :type vector: list
         :return: Response from the BagelDB API in json format.
         :rtype: dict
         """
         if not isinstance(vector, list):
             raise ValueError("Vector must be an array")
 
+        headers = {'Content-Type': 'application/json'}
+
         data = {
             "index": self.index,
             "vector": vector
         }
 
         try:
-            response = requests.post(f'{self.baseURL}/v0/search', data=json.dumps(data))
+            response = requests.post(f'{self.baseURL}/v0/search', headers=headers, data=json.dumps(data))
             response.raise_for_status()
             return response.json()
         except requests.exceptions.RequestException as err:
             print(f'Request failed: {err}')
 
     def insertFromTexts(self, texts, model='text-embedding-ada-002'):
         """
@@ -131,18 +136,18 @@
         :rtype: dict
         """
         if not isinstance(texts, list):
             raise ValueError("Texts must be a list")
 
         vectors = []
         for i, text in enumerate(texts):
-            embedding = self.getOpenAIEmbedding(text, model)
+            embedding = self.getOpenAIEmbedding(text, model)['data'][0]
             vector = {
                 'id': f'vec{i}',
-                'values': embedding['embeddings'],
+                'values': embedding['embedding'],
                 'metadata': {'text': text},
             }
             vectors.append(vector)
 
         return self.insert(vectors)
 
     def searchFromText(self, text, model='text-embedding-ada-002'):
@@ -155,12 +160,12 @@
         :type model: str, optional
         :return: Response from the BagelDB API in json format.
         :rtype: dict
         """
         if not isinstance(text, str):
             raise ValueError("Text must be a string")
 
-        embedding = self.getOpenAIEmbedding(text, model)
-        vector = embedding['embeddings']
+        embedding = self.getOpenAIEmbedding(text, model)['data'][0]
+        vector = embedding['embedding']
 
         return self.search(vector)
```

### Comparing `betabageldb-0.1.4/PKG-INFO` & `betabageldb-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.1.4
+Version: 0.1.5
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `betabageldb-0.1.4/README.md` & `betabageldb-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.4/betabageldb.egg-info/PKG-INFO` & `betabageldb-0.1.5/betabageldb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.1.4
+Version: 0.1.5
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `betabageldb-0.1.4/setup.py` & `betabageldb-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="betabageldb",
-    version="0.1.4",
+    version="0.1.5",
     description="BagelDB is a Python library for interacting with the BagelDB API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bidhan Roy",
     author_email="bidhan@bageldb.ai",
     url="https://github.com/Bagel-DB/Client",
     py_modules=["BagelDB"],
```


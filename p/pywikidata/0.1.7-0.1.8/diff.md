# Comparing `tmp/pywikidata-0.1.7.tar.gz` & `tmp/pywikidata-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywikidata-0.1.7.tar", max compression
+gzip compressed data, was "pywikidata-0.1.8.tar", max compression
```

## Comparing `pywikidata-0.1.7.tar` & `pywikidata-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1084 2023-01-24 13:42:24.565442 pywikidata-0.1.7/LICENSE
--rw-r--r--   0        0        0      732 2023-01-25 13:20:25.687181 pywikidata-0.1.7/README.md
--rw-r--r--   0        0        0      393 2023-02-21 11:05:38.285589 pywikidata-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       27 2023-01-25 09:02:52.892236 pywikidata-0.1.7/pywikidata/__init__.py
--rw-r--r--   0        0        0      218 2023-01-25 09:11:19.262671 pywikidata-0.1.7/pywikidata/config.py
--rw-r--r--   0        0        0    11300 2023-02-21 11:10:33.481968 pywikidata-0.1.7/pywikidata/entity.py
--rw-r--r--   0        0        0     1278 2023-01-24 13:52:17.436119 pywikidata-0.1.7/pywikidata/logger.py
--rw-r--r--   0        0        0     3280 2023-02-21 11:06:17.467092 pywikidata-0.1.7/pywikidata/utils.py
--rw-r--r--   0        0        0     1408 1970-01-01 00:00:00.000000 pywikidata-0.1.7/setup.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 pywikidata-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-01-24 13:42:24.565442 pywikidata-0.1.8/LICENSE
+-rw-r--r--   0        0        0      732 2023-01-25 13:20:25.687181 pywikidata-0.1.8/README.md
+-rw-r--r--   0        0        0      393 2023-07-03 19:33:44.207773 pywikidata-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-01-25 09:02:52.892236 pywikidata-0.1.8/pywikidata/__init__.py
+-rw-r--r--   0        0        0     2009 2023-07-03 19:32:28.539113 pywikidata-0.1.8/pywikidata/attributes.py
+-rw-r--r--   0        0        0      293 2023-07-03 19:15:37.834641 pywikidata-0.1.8/pywikidata/config.py
+-rw-r--r--   0        0        0    11404 2023-07-03 19:27:26.892043 pywikidata-0.1.8/pywikidata/entity.py
+-rw-r--r--   0        0        0     1278 2023-01-24 13:52:17.436119 pywikidata-0.1.8/pywikidata/logger.py
+-rw-r--r--   0        0        0     3267 2023-07-03 19:32:28.560016 pywikidata-0.1.8/pywikidata/utils.py
+-rw-r--r--   0        0        0     1408 1970-01-01 00:00:00.000000 pywikidata-0.1.8/setup.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 pywikidata-0.1.8/PKG-INFO
```

### Comparing `pywikidata-0.1.7/LICENSE` & `pywikidata-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pywikidata-0.1.7/README.md` & `pywikidata-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pywikidata-0.1.7/pywikidata/entity.py` & `pywikidata-0.1.8/pywikidata/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 from .utils import request_to_wikidata
+from .attributes import _WikidataAttributes
 
 
 class _WikiDataBase:
     @staticmethod
     def _entity_uri_to_id(uri):
         return uri.split("/")[-1]
 
@@ -210,14 +211,15 @@
             self._description = None
             self._image = None
             self._forward_one_hop_neighbours = None
             self._backward_one_hop_neighbours = None
             self._instance_of = None
             self._subclass_of = None
             self.is_property = self.idx[0] == "P"
+            self.attributes = _WikidataAttributes(self.idx)
 
     @classmethod
     def from_label(cls, label: str):
         """
         Returns list of entities with corresponding label
         """
         responce = cls._request_entity_by_label(label)
```

### Comparing `pywikidata-0.1.7/pywikidata/logger.py` & `pywikidata-0.1.8/pywikidata/logger.py`

 * *Files identical despite different names*

### Comparing `pywikidata-0.1.7/pywikidata/utils.py` & `pywikidata-0.1.8/pywikidata/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,48 +73,46 @@
         raise e
 
 
 @memory.cache
 def get_wd_search_results(
     search_string: str,
     max_results: int = 500,
-    language: str = 'en',
+    language: str = "en",
     mediawiki_api_url: str = "https://www.wikidata.org/w/api.php",
     user_agent: str = None,
 ) -> list:
     params = {
-        'action': 'wbsearchentities',
-        'language': language,
-        'search': search_string,
-        'format': 'json',
-        'limit': 50
+        "action": "wbsearchentities",
+        "language": language,
+        "search": search_string,
+        "format": "json",
+        "limit": 50,
     }
 
     user_agent = "pywikidata" if user_agent is None else user_agent
-    headers = {
-        'User-Agent': user_agent
-    }
+    headers = {"User-Agent": user_agent}
 
     cont_count = 1
     results = []
     while cont_count > 0:
-        params.update({'continue': 0 if cont_count == 1 else cont_count})
+        params.update({"continue": 0 if cont_count == 1 else cont_count})
 
         reply = requests.get(mediawiki_api_url, params=params, headers=headers)
         reply.raise_for_status()
         search_results = reply.json()
 
-        if search_results['success'] != 1:
-            raise Exception('WD search failed')
+        if search_results["success"] != 1:
+            raise Exception("WD search failed")
         else:
-            for i in search_results['search']:
-                results.append(i['id'])
+            for i in search_results["search"]:
+                results.append(i["id"])
 
-        if 'search-continue' not in search_results:
+        if "search-continue" not in search_results:
             cont_count = 0
         else:
-            cont_count = search_results['search-continue']
+            cont_count = search_results["search-continue"]
 
         if cont_count > max_results:
             break
 
     return results
```

### Comparing `pywikidata-0.1.7/setup.py` & `pywikidata-0.1.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['joblib>=1.2.0,<2.0.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'pywikidata',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Python Wrapper for Wikidata KG',
     'long_description': '# pyWikiData\n\nPython wrapper for Wikidata Knowledge Graph\n\nSupported SPARQL backend\n\n## Install\n\n```bash\npip install pywikidata\n```\n\n#### Install from source by poetry\n```bash\npoetry build\n```\n\n## Usage\n```python\nfrom pywikidata import Entity\n\nentity = Entity(\'Q90\')\nentity.label # >> Paris\n\nEntity.from_label(\'Paris\') # >> [<Entity: Q116373885>, <Entity: Q116373939>, <Entity: Q90>, ...]\n\nentity.instance_of # >> [<Entity: Q174844>, <Entity: Q200250>, <Entity: Q208511>, ...]\n\nentity.forward_one_hop_neighbours # >> [(<Entity(Property): P6>, <Entity: Q2851133>), (<Entity(Property): P8138>, <Entity: Q108921672>), ...]\nentity.backward_one_hop_neighbours\n\nEntity("P81").is_property # >> True\nEntity("Q90").is_property # >> False\n```',
     'author': 'Mikhail Salnikov',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pywikidata-0.1.7/PKG-INFO` & `pywikidata-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikidata
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python Wrapper for Wikidata KG
 License: MIT
 Author: Mikhail Salnikov
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```


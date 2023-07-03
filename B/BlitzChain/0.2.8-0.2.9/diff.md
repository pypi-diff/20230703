# Comparing `tmp/BlitzChain-0.2.8.tar.gz` & `tmp/BlitzChain-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlitzChain-0.2.8.tar", last modified: Sun Jul  2 07:43:14 2023, max compression
+gzip compressed data, was "BlitzChain-0.2.9.tar", last modified: Mon Jul  3 09:49:36 2023, max compression
```

## Comparing `BlitzChain-0.2.8.tar` & `BlitzChain-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-02 07:43:14.634204 BlitzChain-0.2.8/
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-02 07:43:14.629951 BlitzChain-0.2.8/BlitzChain.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-02 07:43:14.000000 BlitzChain-0.2.8/BlitzChain.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-02 07:43:14.000000 BlitzChain-0.2.8/BlitzChain.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-02 07:43:14.000000 BlitzChain-0.2.8/BlitzChain.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-02 07:43:14.000000 BlitzChain-0.2.8/BlitzChain.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-02 07:43:14.000000 BlitzChain-0.2.8/BlitzChain.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.2.8/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-02 07:43:14.633931 BlitzChain-0.2.8/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-06-25 07:25:46.000000 BlitzChain-0.2.8/README.md
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-02 07:43:14.631242 BlitzChain-0.2.8/blitzchain/
--rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-02 07:43:10.000000 BlitzChain-0.2.8/blitzchain/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     5546 2023-07-02 07:43:05.000000 BlitzChain-0.2.8/blitzchain/api.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2138 2023-06-28 05:25:25.000000 BlitzChain-0.2.8/blitzchain/splitter.py
--rw-r--r--   0 jackywong   (501) staff       (20)      763 2023-06-28 00:10:27.000000 BlitzChain-0.2.8/blitzchain/utils.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-02 07:43:14.631908 BlitzChain-0.2.8/cli/
--rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-06-28 03:39:00.000000 BlitzChain-0.2.8/cli/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)      430 2023-06-28 13:19:06.000000 BlitzChain-0.2.8/cli/main.py
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-02 07:43:14.634285 BlitzChain-0.2.8/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      485 2023-06-28 05:27:42.000000 BlitzChain-0.2.8/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-02 07:43:14.633334 BlitzChain-0.2.8/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.2.8/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.2.8/tests/test_pdf.py
--rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.2.8/tests/test_qa.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-03 09:49:36.544503 BlitzChain-0.2.9/
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-03 09:49:36.542070 BlitzChain-0.2.9/BlitzChain.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-03 09:49:36.000000 BlitzChain-0.2.9/BlitzChain.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-03 09:49:36.000000 BlitzChain-0.2.9/BlitzChain.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-03 09:49:36.000000 BlitzChain-0.2.9/BlitzChain.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-03 09:49:36.000000 BlitzChain-0.2.9/BlitzChain.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-03 09:49:36.000000 BlitzChain-0.2.9/BlitzChain.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.2.9/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-03 09:49:36.544365 BlitzChain-0.2.9/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-06-25 07:25:46.000000 BlitzChain-0.2.9/README.md
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-03 09:49:36.542648 BlitzChain-0.2.9/blitzchain/
+-rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-03 09:49:25.000000 BlitzChain-0.2.9/blitzchain/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     5570 2023-07-03 09:49:07.000000 BlitzChain-0.2.9/blitzchain/api.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2138 2023-07-03 09:49:17.000000 BlitzChain-0.2.9/blitzchain/splitter.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      763 2023-06-28 00:10:27.000000 BlitzChain-0.2.9/blitzchain/utils.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-03 09:49:36.543204 BlitzChain-0.2.9/cli/
+-rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-06-28 03:39:00.000000 BlitzChain-0.2.9/cli/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      430 2023-06-28 13:19:06.000000 BlitzChain-0.2.9/cli/main.py
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-03 09:49:36.544553 BlitzChain-0.2.9/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      485 2023-06-28 05:27:42.000000 BlitzChain-0.2.9/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-03 09:49:36.544085 BlitzChain-0.2.9/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.2.9/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.2.9/tests/test_pdf.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.2.9/tests/test_qa.py
```

### Comparing `BlitzChain-0.2.8/LICENSE` & `BlitzChain-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.2.8/README.md` & `BlitzChain-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.2.8/blitzchain/api.py` & `BlitzChain-0.2.9/blitzchain/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """The API behind BlitzChain
 """
 import requests
+from typing import List
 from .splitter import WordSplitter
 
 def get_json_response(response):
     try:
         return response.json()
     except Exception as e:
         return response.content
```

### Comparing `BlitzChain-0.2.8/blitzchain/splitter.py` & `BlitzChain-0.2.9/blitzchain/splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 from typing import List, Dict
 
 class WordSplitter:
     def split_text_into_array(
         self, text: str, max_word_count: int = 200, overlap: int = 10,
         chunksize: int=20
-    ) -> list[str]:
+    ) -> List[str]:
         """Splits the input text into an array of strings with each element not exceeding the specified max_word_count. Allows an overlapping number of words."""
         words = text.split()
         word_count = len(words)
 
         if word_count <= max_word_count:
             yield [text]
 
@@ -32,15 +32,15 @@
     def split_object_text(
         self,
         dicts: List[Dict],
         key: str,
         max_word_count: int = 200,
         overlap: int = 10,
         chunksize: int=20
-    ) -> list[dict]:
+    ) -> List[dict]:
         """Splits the text of a specified key in a list of dictionaries, creating a new dictionary for each split text segment."""
         print("splitting text...")
         split_dicts = []
         for d in dicts:
             if key in d:
                 text = d[key]
                 print("split array")
```

### Comparing `BlitzChain-0.2.8/blitzchain/utils.py` & `BlitzChain-0.2.9/blitzchain/utils.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.2.8/tests/test_pdf.py` & `BlitzChain-0.2.9/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.2.8/tests/test_qa.py` & `BlitzChain-0.2.9/tests/test_qa.py`

 * *Files identical despite different names*


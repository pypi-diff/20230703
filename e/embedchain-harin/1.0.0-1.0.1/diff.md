# Comparing `tmp/embedchain-harin-1.0.0.tar.gz` & `tmp/embedchain-harin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/embedchain-harin-1.0.0.tar", last modified: Sat Jul  1 23:43:37 2023, max compression
+gzip compressed data, was "dist/embedchain-harin-1.0.1.tar", last modified: Mon Jul  3 02:35:45 2023, max compression
```

## Comparing `embedchain-harin-1.0.0.tar` & `embedchain-harin-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 harin     (1000) harin     (1000)        0 2023-07-01 23:43:37.443641 embedchain-harin-1.0.0/
--rw-rw-r--   0 harin     (1000) harin     (1000)     9041 2023-07-01 23:43:37.443641 embedchain-harin-1.0.0/PKG-INFO
--rw-rw-r--   0 harin     (1000) harin     (1000)     7084 2023-07-01 23:26:51.000000 embedchain-harin-1.0.0/README.md
-drwxrwxr-x   0 harin     (1000) harin     (1000)        0 2023-07-01 23:43:37.443641 embedchain-harin-1.0.0/embedchain/
--rw-rw-r--   0 harin     (1000) harin     (1000)       27 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/__init__.py
-drwxrwxr-x   0 harin     (1000) harin     (1000)        0 2023-07-01 23:43:37.443641 embedchain-harin-1.0.0/embedchain/chunkers/
--rw-rw-r--   0 harin     (1000) harin     (1000)        0 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/chunkers/__init__.py
--rw-rw-r--   0 harin     (1000) harin     (1000)      819 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/chunkers/base_chunker.py
--rw-rw-r--   0 harin     (1000) harin     (1000)      421 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/chunkers/pdf_file.py
--rw-rw-r--   0 harin     (1000) harin     (1000)      421 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/chunkers/qna_pair.py
--rw-rw-r--   0 harin     (1000) harin     (1000)      418 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/chunkers/text.py
--rw-rw-r--   0 harin     (1000) harin     (1000)      421 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/chunkers/web_page.py
--rw-rw-r--   0 harin     (1000) harin     (1000)      426 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/chunkers/youtube_video.py
--rw-rw-r--   0 harin     (1000) harin     (1000)     9147 2023-07-01 22:37:02.000000 embedchain-harin-1.0.0/embedchain/embedchain.py
-drwxrwxr-x   0 harin     (1000) harin     (1000)        0 2023-07-01 23:43:37.443641 embedchain-harin-1.0.0/embedchain/loaders/
--rw-rw-r--   0 harin     (1000) harin     (1000)        0 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/loaders/__init__.py
--rw-rw-r--   0 harin     (1000) harin     (1000)      301 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/loaders/local_qna_pair.py
--rw-rw-r--   0 harin     (1000) harin     (1000)      215 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/loaders/local_text.py
--rw-rw-r--   0 harin     (1000) harin     (1000)      639 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/loaders/pdf_file.py
--rw-rw-r--   0 harin     (1000) harin     (1000)      731 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/loaders/web_page.py
--rw-rw-r--   0 harin     (1000) harin     (1000)      618 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/loaders/youtube_video.py
--rw-rw-r--   0 harin     (1000) harin     (1000)     1162 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/utils.py
-drwxrwxr-x   0 harin     (1000) harin     (1000)        0 2023-07-01 23:43:37.443641 embedchain-harin-1.0.0/embedchain/vectordb/
--rw-rw-r--   0 harin     (1000) harin     (1000)        0 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/vectordb/__init__.py
--rw-rw-r--   0 harin     (1000) harin     (1000)      293 2023-06-30 19:11:32.000000 embedchain-harin-1.0.0/embedchain/vectordb/base_vector_db.py
--rw-rw-r--   0 harin     (1000) harin     (1000)     1099 2023-07-01 22:32:21.000000 embedchain-harin-1.0.0/embedchain/vectordb/chroma_db.py
-drwxrwxr-x   0 harin     (1000) harin     (1000)        0 2023-07-01 23:43:37.443641 embedchain-harin-1.0.0/embedchain_harin.egg-info/
--rw-rw-r--   0 harin     (1000) harin     (1000)     9041 2023-07-01 23:43:37.000000 embedchain-harin-1.0.0/embedchain_harin.egg-info/PKG-INFO
--rw-rw-r--   0 harin     (1000) harin     (1000)      816 2023-07-01 23:43:37.000000 embedchain-harin-1.0.0/embedchain_harin.egg-info/SOURCES.txt
--rw-rw-r--   0 harin     (1000) harin     (1000)        1 2023-07-01 23:43:37.000000 embedchain-harin-1.0.0/embedchain_harin.egg-info/dependency_links.txt
--rw-rw-r--   0 harin     (1000) harin     (1000)      141 2023-07-01 23:43:37.000000 embedchain-harin-1.0.0/embedchain_harin.egg-info/requires.txt
--rw-rw-r--   0 harin     (1000) harin     (1000)       11 2023-07-01 23:43:37.000000 embedchain-harin-1.0.0/embedchain_harin.egg-info/top_level.txt
--rw-rw-r--   0 harin     (1000) harin     (1000)       38 2023-07-01 23:43:37.443641 embedchain-harin-1.0.0/setup.cfg
--rw-rw-r--   0 harin     (1000) harin     (1000)     1036 2023-07-01 23:41:32.000000 embedchain-harin-1.0.0/setup.py
+drwxrwxr-x   0 harin     (1000) harin     (1000)        0 2023-07-03 02:35:45.557619 embedchain-harin-1.0.1/
+-rw-rw-r--   0 harin     (1000) harin     (1000)     9041 2023-07-03 02:35:45.557619 embedchain-harin-1.0.1/PKG-INFO
+-rw-rw-r--   0 harin     (1000) harin     (1000)     7084 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/README.md
+drwxrwxr-x   0 harin     (1000) harin     (1000)        0 2023-07-03 02:35:45.553619 embedchain-harin-1.0.1/embedchain/
+-rw-rw-r--   0 harin     (1000) harin     (1000)       27 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/__init__.py
+drwxrwxr-x   0 harin     (1000) harin     (1000)        0 2023-07-03 02:35:45.553619 embedchain-harin-1.0.1/embedchain/chunkers/
+-rw-rw-r--   0 harin     (1000) harin     (1000)        0 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/chunkers/__init__.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)      819 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/chunkers/base_chunker.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)      421 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/chunkers/pdf_file.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)      421 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/chunkers/qna_pair.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)      418 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/chunkers/text.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)      421 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/chunkers/web_page.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)      426 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/chunkers/youtube_video.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)     9109 2023-07-02 22:12:19.000000 embedchain-harin-1.0.1/embedchain/embedchain.py
+drwxrwxr-x   0 harin     (1000) harin     (1000)        0 2023-07-03 02:35:45.557619 embedchain-harin-1.0.1/embedchain/loaders/
+-rw-rw-r--   0 harin     (1000) harin     (1000)        0 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/loaders/__init__.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)      301 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/loaders/local_qna_pair.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)      215 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/loaders/local_text.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)      639 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/loaders/pdf_file.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)      731 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/loaders/web_page.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)      618 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/loaders/youtube_video.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)     1162 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/utils.py
+drwxrwxr-x   0 harin     (1000) harin     (1000)        0 2023-07-03 02:35:45.557619 embedchain-harin-1.0.1/embedchain/vectordb/
+-rw-rw-r--   0 harin     (1000) harin     (1000)        0 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/vectordb/__init__.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)      293 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/vectordb/base_vector_db.py
+-rw-rw-r--   0 harin     (1000) harin     (1000)     1099 2023-07-02 18:28:00.000000 embedchain-harin-1.0.1/embedchain/vectordb/chroma_db.py
+drwxrwxr-x   0 harin     (1000) harin     (1000)        0 2023-07-03 02:35:45.557619 embedchain-harin-1.0.1/embedchain_harin.egg-info/
+-rw-rw-r--   0 harin     (1000) harin     (1000)     9041 2023-07-03 02:35:45.000000 embedchain-harin-1.0.1/embedchain_harin.egg-info/PKG-INFO
+-rw-rw-r--   0 harin     (1000) harin     (1000)      816 2023-07-03 02:35:45.000000 embedchain-harin-1.0.1/embedchain_harin.egg-info/SOURCES.txt
+-rw-rw-r--   0 harin     (1000) harin     (1000)        1 2023-07-03 02:35:45.000000 embedchain-harin-1.0.1/embedchain_harin.egg-info/dependency_links.txt
+-rw-rw-r--   0 harin     (1000) harin     (1000)      141 2023-07-03 02:35:45.000000 embedchain-harin-1.0.1/embedchain_harin.egg-info/requires.txt
+-rw-rw-r--   0 harin     (1000) harin     (1000)       11 2023-07-03 02:35:45.000000 embedchain-harin-1.0.1/embedchain_harin.egg-info/top_level.txt
+-rw-rw-r--   0 harin     (1000) harin     (1000)       38 2023-07-03 02:35:45.557619 embedchain-harin-1.0.1/setup.cfg
+-rw-rw-r--   0 harin     (1000) harin     (1000)     1036 2023-07-03 02:35:39.000000 embedchain-harin-1.0.1/setup.py
```

### Comparing `embedchain-harin-1.0.0/PKG-INFO` & `embedchain-harin-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedchain-harin
-Version: 1.0.0
+Version: 1.0.1
 Summary: embedchain is a framework to easily create LLM powered bots over any dataset
 Home-page: https://github.com/harin329/embedchain
 Author: Harin Wu
 Author-email: harinwu99@gmail.com
 License: UNKNOWN
 Description: # embedchain
```

### Comparing `embedchain-harin-1.0.0/README.md` & `embedchain-harin-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `embedchain-harin-1.0.0/embedchain/chunkers/base_chunker.py` & `embedchain-harin-1.0.1/embedchain/chunkers/base_chunker.py`

 * *Files identical despite different names*

### Comparing `embedchain-harin-1.0.0/embedchain/embedchain.py` & `embedchain-harin-1.0.1/embedchain/embedchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,18 +207,18 @@
         """
         Generates a prompt based on the given query and context, ready to be passed to an LLM
 
         :param input_query: The query to use.
         :param context: Similar documents to the query used as context.
         :return: The prompt
         """
-        prompt = f"""Use the following pieces of context to answer the query at the end. If you don't know the answer, just say that you don't know, don't try to make up an answer.
+        prompt = f"""Use the following pieces of context to continue the conversation as {os.getenv("BOT_IS")}.
         {context}
-        Query: {input_query}
-        Helpful Answer:
+        {os.getenv("BOT_TALKING_TO")}: {input_query}
+        {os.getenv("BOT_IS")}:
         """
         return prompt
 
     def get_answer_from_llm(self, prompt):
         """
         Gets an answer based on the given query and context by passing it
         to an LLM.
```

### Comparing `embedchain-harin-1.0.0/embedchain/loaders/pdf_file.py` & `embedchain-harin-1.0.1/embedchain/loaders/pdf_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-harin-1.0.0/embedchain/loaders/web_page.py` & `embedchain-harin-1.0.1/embedchain/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `embedchain-harin-1.0.0/embedchain/loaders/youtube_video.py` & `embedchain-harin-1.0.1/embedchain/loaders/youtube_video.py`

 * *Files identical despite different names*

### Comparing `embedchain-harin-1.0.0/embedchain/utils.py` & `embedchain-harin-1.0.1/embedchain/utils.py`

 * *Files identical despite different names*

### Comparing `embedchain-harin-1.0.0/embedchain/vectordb/chroma_db.py` & `embedchain-harin-1.0.1/embedchain/vectordb/chroma_db.py`

 * *Files identical despite different names*

### Comparing `embedchain-harin-1.0.0/embedchain_harin.egg-info/PKG-INFO` & `embedchain-harin-1.0.1/embedchain_harin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedchain-harin
-Version: 1.0.0
+Version: 1.0.1
 Summary: embedchain is a framework to easily create LLM powered bots over any dataset
 Home-page: https://github.com/harin329/embedchain
 Author: Harin Wu
 Author-email: harinwu99@gmail.com
 License: UNKNOWN
 Description: # embedchain
```

### Comparing `embedchain-harin-1.0.0/embedchain_harin.egg-info/SOURCES.txt` & `embedchain-harin-1.0.1/embedchain_harin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embedchain-harin-1.0.0/setup.py` & `embedchain-harin-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="embedchain-harin",
-    version="1.0.0",
+    version="1.0.1",
     author="Harin Wu",
     author_email="harinwu99@gmail.com",
     description="embedchain is a framework to easily create LLM powered bots over any dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/harin329/embedchain",
     packages=setuptools.find_packages(),
```


# Comparing `tmp/llm-to-corpus-0.0.1.tar.gz` & `tmp/llm-to-corpus-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-to-corpus-0.0.1.tar", last modified: Mon Jul  3 20:39:58 2023, max compression
+gzip compressed data, was "llm-to-corpus-0.0.2.tar", last modified: Mon Jul  3 20:49:16 2023, max compression
```

## Comparing `llm-to-corpus-0.0.1.tar` & `llm-to-corpus-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-03 20:39:58.057297 llm-to-corpus-0.0.1/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-06-10 18:10:04.000000 llm-to-corpus-0.0.1/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2129 2023-07-03 20:39:58.057297 llm-to-corpus-0.0.1/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1521 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.1/README.md
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-03 20:39:58.057297 llm-to-corpus-0.0.1/llm_to_corpus.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2129 2023-07-03 20:39:58.000000 llm-to-corpus-0.0.1/llm_to_corpus.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      398 2023-07-03 20:39:58.000000 llm-to-corpus-0.0.1/llm_to_corpus.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-07-03 20:39:58.000000 llm-to-corpus-0.0.1/llm_to_corpus.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       61 2023-07-03 20:39:58.000000 llm-to-corpus-0.0.1/llm_to_corpus.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       37 2023-07-03 20:39:58.000000 llm-to-corpus-0.0.1/llm_to_corpus.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       18 2023-07-03 20:39:58.000000 llm-to-corpus-0.0.1/llm_to_corpus.egg-info/top_level.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-07-03 20:39:58.057297 llm-to-corpus-0.0.1/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1221 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.1/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-03 20:39:58.057297 llm-to-corpus-0.0.1/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-03 20:39:58.057297 llm-to-corpus-0.0.1/src/llm_to_corpus/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1405 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.1/src/llm_to_corpus/bloom.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1215 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.1/src/llm_to_corpus/chatgpt.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3341 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.1/src/llm_to_corpus/cli.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      931 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.1/src/llm_to_corpus/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.1/src/llm_to_corpus/version.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-03 20:49:16.900550 llm-to-corpus-0.0.2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-06-10 18:10:04.000000 llm-to-corpus-0.0.2/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2258 2023-07-03 20:49:16.900550 llm-to-corpus-0.0.2/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1657 2023-07-03 20:42:55.000000 llm-to-corpus-0.0.2/README.md
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-03 20:49:16.896550 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2258 2023-07-03 20:49:16.000000 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      398 2023-07-03 20:49:16.000000 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-07-03 20:49:16.000000 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       61 2023-07-03 20:49:16.000000 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       37 2023-07-03 20:49:16.000000 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       18 2023-07-03 20:49:16.000000 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/top_level.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-07-03 20:49:16.900550 llm-to-corpus-0.0.2/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1214 2023-07-03 20:45:37.000000 llm-to-corpus-0.0.2/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-03 20:49:16.896550 llm-to-corpus-0.0.2/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-03 20:49:16.900550 llm-to-corpus-0.0.2/src/llm_to_corpus/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1405 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.2/src/llm_to_corpus/bloom.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1215 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.2/src/llm_to_corpus/chatgpt.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3341 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.2/src/llm_to_corpus/cli.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      931 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.2/src/llm_to_corpus/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-07-03 20:46:18.000000 llm-to-corpus-0.0.2/src/llm_to_corpus/version.py
```

### Comparing `llm-to-corpus-0.0.1/LICENSE` & `llm-to-corpus-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-to-corpus-0.0.1/PKG-INFO` & `llm-to-corpus-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: llm-to-corpus
-Version: 0.0.1
+Version: 0.0.2
 Summary: Large language model to corpus
-Home-page: https://github.com/Softcatala/whisper-ctranslate2
+Home-page: https://github.com/jordimas/llm-to-corpus/
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
+[![PyPI version](https://img.shields.io/pypi/v/llm-to-corpus.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/llm-to-corpus/)
+
 # Introduction
 
 The goal of this tool is to apply Large Language Models operations to monolingual corpus to generate parallell corpus.
 
 Uses cases:
 
 * Asking a model to translate, summarize, paraphrasing original sentence to be able to benchmark its performance
```

### Comparing `llm-to-corpus-0.0.1/README.md` & `llm-to-corpus-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![PyPI version](https://img.shields.io/pypi/v/llm-to-corpus.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/llm-to-corpus/)
+
 # Introduction
 
 The goal of this tool is to apply Large Language Models operations to monolingual corpus to generate parallell corpus.
 
 Uses cases:
 
 * Asking a model to translate, summarize, paraphrasing original sentence to be able to benchmark its performance
```

### Comparing `llm-to-corpus-0.0.1/llm_to_corpus.egg-info/PKG-INFO` & `llm-to-corpus-0.0.2/llm_to_corpus.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: llm-to-corpus
-Version: 0.0.1
+Version: 0.0.2
 Summary: Large language model to corpus
-Home-page: https://github.com/Softcatala/whisper-ctranslate2
+Home-page: https://github.com/jordimas/llm-to-corpus/
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
+[![PyPI version](https://img.shields.io/pypi/v/llm-to-corpus.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/llm-to-corpus/)
+
 # Introduction
 
 The goal of this tool is to apply Large Language Models operations to monolingual corpus to generate parallell corpus.
 
 Uses cases:
 
 * Asking a model to translate, summarize, paraphrasing original sentence to be able to benchmark its performance
```

### Comparing `llm-to-corpus-0.0.1/setup.py` & `llm-to-corpus-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name="llm-to-corpus",
     version=read_version(),
     description="Large language model to corpus",
     long_description=README,
     long_description_content_type="text/markdown",
-    url="https://github.com/Softcatala/whisper-ctranslate2",
+    url="https://github.com/jordimas/llm-to-corpus/",
     author="Jordi Mas",
     author_email="jmas@softcatala.org",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `llm-to-corpus-0.0.1/src/llm_to_corpus/bloom.py` & `llm-to-corpus-0.0.2/src/llm_to_corpus/bloom.py`

 * *Files identical despite different names*

### Comparing `llm-to-corpus-0.0.1/src/llm_to_corpus/chatgpt.py` & `llm-to-corpus-0.0.2/src/llm_to_corpus/chatgpt.py`

 * *Files identical despite different names*

### Comparing `llm-to-corpus-0.0.1/src/llm_to_corpus/cli.py` & `llm-to-corpus-0.0.2/src/llm_to_corpus/cli.py`

 * *Files identical despite different names*

### Comparing `llm-to-corpus-0.0.1/src/llm_to_corpus/models.py` & `llm-to-corpus-0.0.2/src/llm_to_corpus/models.py`

 * *Files identical despite different names*


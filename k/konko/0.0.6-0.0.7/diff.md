# Comparing `tmp/konko-0.0.6.tar.gz` & `tmp/konko-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konko-0.0.6.tar", last modified: Sun Jul  2 20:00:17 2023, max compression
+gzip compressed data, was "konko-0.0.7.tar", last modified: Mon Jul  3 02:40:17 2023, max compression
```

## Comparing `konko-0.0.6.tar` & `konko-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-02 20:00:17.760256 konko-0.0.6/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-07-02 20:00:17.760125 konko-0.0.6/PKG-INFO
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       29 2023-06-01 17:28:19.000000 konko-0.0.6/README.md
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      304 2023-07-02 19:59:48.000000 konko-0.0.6/pyproject.toml
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       38 2023-07-02 20:00:17.760303 konko-0.0.6/setup.cfg
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-02 20:00:17.758551 konko-0.0.6/src/
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-02 20:00:17.759288 konko-0.0.6/src/konko/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      119 2023-07-01 02:14:31.000000 konko-0.0.6/src/konko/__init__.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)     1887 2023-06-15 22:41:35.000000 konko-0.0.6/src/konko/evaluate.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)     4296 2023-07-01 02:13:25.000000 konko-0.0.6/src/konko/generate.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)     1277 2023-07-01 02:14:39.000000 konko-0.0.6/src/konko/models.py
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-02 20:00:17.759971 konko-0.0.6/src/konko/utils/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       41 2023-06-30 21:50:53.000000 konko-0.0.6/src/konko/utils/constants.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      209 2023-06-30 22:20:34.000000 konko-0.0.6/src/konko/utils/utils.py
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-02 20:00:17.759758 konko-0.0.6/src/konko.egg-info/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-07-02 20:00:17.000000 konko-0.0.6/src/konko.egg-info/PKG-INFO
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      296 2023-07-02 20:00:17.000000 konko-0.0.6/src/konko.egg-info/SOURCES.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-07-02 20:00:17.000000 konko-0.0.6/src/konko.egg-info/dependency_links.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        6 2023-07-02 20:00:17.000000 konko-0.0.6/src/konko.egg-info/top_level.txt
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 02:40:17.805166 konko-0.0.7/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-07-03 02:40:17.805037 konko-0.0.7/PKG-INFO
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       29 2023-06-01 17:28:19.000000 konko-0.0.7/README.md
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      304 2023-07-03 02:39:47.000000 konko-0.0.7/pyproject.toml
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       38 2023-07-03 02:40:17.805204 konko-0.0.7/setup.cfg
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 02:40:17.803429 konko-0.0.7/src/
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 02:40:17.804174 konko-0.0.7/src/konko/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      119 2023-07-01 02:14:31.000000 konko-0.0.7/src/konko/__init__.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)     1887 2023-06-15 22:41:35.000000 konko-0.0.7/src/konko/evaluate.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)     4305 2023-07-03 02:37:55.000000 konko-0.0.7/src/konko/generate.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)     1277 2023-07-01 02:14:39.000000 konko-0.0.7/src/konko/models.py
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 02:40:17.804904 konko-0.0.7/src/konko/utils/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      119 2023-07-02 20:04:21.000000 konko-0.0.7/src/konko/utils/__init__.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       41 2023-06-30 21:50:53.000000 konko-0.0.7/src/konko/utils/constants.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      209 2023-06-30 22:20:34.000000 konko-0.0.7/src/konko/utils/utils.py
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 02:40:17.804584 konko-0.0.7/src/konko.egg-info/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-07-03 02:40:17.000000 konko-0.0.7/src/konko.egg-info/PKG-INFO
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      324 2023-07-03 02:40:17.000000 konko-0.0.7/src/konko.egg-info/SOURCES.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-07-03 02:40:17.000000 konko-0.0.7/src/konko.egg-info/dependency_links.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)        6 2023-07-03 02:40:17.000000 konko-0.0.7/src/konko.egg-info/top_level.txt
```

### Comparing `konko-0.0.6/src/konko/evaluate.py` & `konko-0.0.7/src/konko/evaluate.py`

 * *Files identical despite different names*

### Comparing `konko-0.0.6/src/konko/generate.py` & `konko-0.0.7/src/konko/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import requests
 import json 
-from utils.constants import TIMEOUT
+from konko.utils.constants import TIMEOUT
+from konko.utils.utils import BackendError
 from typing import Any, Dict, List, Union, Iterator
-from utils.traceback import BackendError
+
 
 def generate(prompt: List[str] = None, 
              models: List[str] = ['gpt-4', 'mpt-7b-instruct', 'llama-30b'],
              prompt_file: str = None,
              prompt_file_separator: str = "----",
              stream: bool = False, 
              optimize: Dict = {"cost" : 10} ) -> Union[List[Dict[str, Union[str, float, int]]],Iterator[Dict[str, Union[str, float, int]]]]:
```

### Comparing `konko-0.0.6/src/konko/models.py` & `konko-0.0.7/src/konko/models.py`

 * *Files identical despite different names*


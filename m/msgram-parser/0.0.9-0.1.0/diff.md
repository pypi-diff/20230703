# Comparing `tmp/msgram-parser-0.0.9.tar.gz` & `tmp/msgram-parser-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram-parser-0.0.9.tar", last modified: Fri Jun 30 13:11:34 2023, max compression
+gzip compressed data, was "msgram-parser-0.1.0.tar", last modified: Mon Jul  3 07:33:03 2023, max compression
```

## Comparing `msgram-parser-0.0.9.tar` & `msgram-parser-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:34.108810 msgram-parser-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-30 13:11:34.108810 msgram-parser-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:34.104810 msgram-parser-0.0.9/genericparser/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/genericparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/genericparser/accept_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/genericparser/genericparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:34.104810 msgram-parser-0.0.9/genericparser/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/genericparser/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:34.104810 msgram-parser-0.0.9/genericparser/plugins/dinamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/genericparser/plugins/dinamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/genericparser/plugins/dinamic/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:34.104810 msgram-parser-0.0.9/genericparser/plugins/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/genericparser/plugins/domain/generic_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:34.104810 msgram-parser-0.0.9/genericparser/plugins/statics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/genericparser/plugins/statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/genericparser/plugins/statics/sonarqube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:34.104810 msgram-parser-0.0.9/genericparser/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/genericparser/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:34.104810 msgram-parser-0.0.9/msgram_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-30 13:11:34.000000 msgram-parser-0.0.9/msgram_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-30 13:11:34.000000 msgram-parser-0.0.9/msgram_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:11:34.000000 msgram-parser-0.0.9/msgram_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 13:11:34.000000 msgram-parser-0.0.9/msgram_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 13:11:34.000000 msgram-parser-0.0.9/msgram_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:11:34.108810 msgram-parser-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:34.104810 msgram-parser-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/tests/test_extract_mettric_sonarqbe.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-30 13:11:13.000000 msgram-parser-0.0.9/tests/tests_main_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:33:03.383514 msgram-parser-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-07-03 07:33:03.383514 msgram-parser-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:33:03.379514 msgram-parser-0.1.0/genericparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/genericparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/genericparser/accept_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/genericparser/genericparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:33:03.379514 msgram-parser-0.1.0/genericparser/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/genericparser/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:33:03.379514 msgram-parser-0.1.0/genericparser/plugins/dinamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/genericparser/plugins/dinamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/genericparser/plugins/dinamic/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:33:03.379514 msgram-parser-0.1.0/genericparser/plugins/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/genericparser/plugins/domain/generic_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:33:03.379514 msgram-parser-0.1.0/genericparser/plugins/statics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/genericparser/plugins/statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/genericparser/plugins/statics/sonarqube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:33:03.379514 msgram-parser-0.1.0/genericparser/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/genericparser/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:33:03.383514 msgram-parser-0.1.0/msgram_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-07-03 07:33:03.000000 msgram-parser-0.1.0/msgram_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-03 07:33:03.000000 msgram-parser-0.1.0/msgram_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 07:33:03.000000 msgram-parser-0.1.0/msgram_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-03 07:33:03.000000 msgram-parser-0.1.0/msgram_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 07:33:03.000000 msgram-parser-0.1.0/msgram_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 07:33:03.383514 msgram-parser-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:33:03.383514 msgram-parser-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/tests/test_extract_mettric_sonarqbe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-03 07:32:46.000000 msgram-parser-0.1.0/tests/tests_main_file.py
```

### Comparing `msgram-parser-0.0.9/LICENSE` & `msgram-parser-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.9/PKG-INFO` & `msgram-parser-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 0.0.9
+Version: 0.1.0
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-0.0.9/README.md` & `msgram-parser-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.9/genericparser/genericparser.py` & `msgram-parser-0.1.0/genericparser/genericparser.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.9/genericparser/plugins/dinamic/github.py` & `msgram-parser-0.1.0/genericparser/plugins/dinamic/github.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os
 from genericparser.plugins.domain.generic_class import GenericStaticABC
 import requests
 
 
 class ParserGithub(GenericStaticABC):
-    token = "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"
+    token = None
+
+    def __init__(self, token=None):
+        self.token = token
 
     def _make_request(self, url, token):
         headers = {
-            "Authorization": f"Bearer {token}",
+            "Authorization": f"Bearer {token}" if token else "",
             "Accept": "application/vnd.github+json",
             "X-GitHub-Api-Version": "2022-11-28",
         }
         try:
             response = requests.get(url, headers=headers)
         except Exception as e:
             print("error making request to github api in url: ", url, e)
```

### Comparing `msgram-parser-0.0.9/genericparser/plugins/domain/generic_class.py` & `msgram-parser-0.1.0/genericparser/plugins/domain/generic_class.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.9/genericparser/plugins/statics/sonarqube.py` & `msgram-parser-0.1.0/genericparser/plugins/statics/sonarqube.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.9/msgram_parser.egg-info/PKG-INFO` & `msgram-parser-0.1.0/msgram_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 0.0.9
+Version: 0.1.0
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-0.0.9/msgram_parser.egg-info/SOURCES.txt` & `msgram-parser-0.1.0/msgram_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.9/pyproject.toml` & `msgram-parser-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram-parser"
-version = "0.0.9"
+version = "0.1.0"
 description = "The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data."
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
```


# Comparing `tmp/spacy-huggingface-hub-0.0.8.tar.gz` & `tmp/spacy-huggingface-hub-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-huggingface-hub-0.0.8.tar", last modified: Thu Dec  8 13:43:44 2022, max compression
+gzip compressed data, was "spacy-huggingface-hub-0.0.9.tar", last modified: Tue Feb  7 16:44:07 2023, max compression
```

## Comparing `spacy-huggingface-hub-0.0.8.tar` & `spacy-huggingface-hub-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-08 13:43:44.096461 spacy-huggingface-hub-0.0.8/
--rw-r--r--   0 vsts      (1001) docker     (122)     1102 2022-12-08 13:43:38.000000 spacy-huggingface-hub-0.0.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)       34 2022-12-08 13:43:38.000000 spacy-huggingface-hub-0.0.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     5340 2022-12-08 13:43:44.096461 spacy-huggingface-hub-0.0.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4567 2022-12-08 13:43:38.000000 spacy-huggingface-hub-0.0.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1066 2022-12-08 13:43:44.096461 spacy-huggingface-hub-0.0.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      182 2022-12-08 13:43:38.000000 spacy-huggingface-hub-0.0.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-08 13:43:44.096461 spacy-huggingface-hub-0.0.8/spacy_huggingface_hub/
--rw-r--r--   0 vsts      (1001) docker     (122)       37 2022-12-08 13:43:38.000000 spacy-huggingface-hub-0.0.8/spacy_huggingface_hub/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      135 2022-12-08 13:43:38.000000 spacy-huggingface-hub-0.0.8/spacy_huggingface_hub/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10801 2022-12-08 13:43:38.000000 spacy-huggingface-hub-0.0.8/spacy_huggingface_hub/push.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-08 13:43:44.096461 spacy-huggingface-hub-0.0.8/spacy_huggingface_hub.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     5340 2022-12-08 13:43:44.000000 spacy-huggingface-hub-0.0.8/spacy_huggingface_hub.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      418 2022-12-08 13:43:44.000000 spacy-huggingface-hub-0.0.8/spacy_huggingface_hub.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2022-12-08 13:43:44.000000 spacy-huggingface-hub-0.0.8/spacy_huggingface_hub.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       82 2022-12-08 13:43:44.000000 spacy-huggingface-hub-0.0.8/spacy_huggingface_hub.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       78 2022-12-08 13:43:44.000000 spacy-huggingface-hub-0.0.8/spacy_huggingface_hub.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       22 2022-12-08 13:43:44.000000 spacy-huggingface-hub-0.0.8/spacy_huggingface_hub.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-07 16:44:07.994889 spacy-huggingface-hub-0.0.9/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1102 2023-02-07 16:44:02.000000 spacy-huggingface-hub-0.0.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-02-07 16:44:02.000000 spacy-huggingface-hub-0.0.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     5340 2023-02-07 16:44:07.994889 spacy-huggingface-hub-0.0.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4567 2023-02-07 16:44:02.000000 spacy-huggingface-hub-0.0.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1059 2023-02-07 16:44:07.994889 spacy-huggingface-hub-0.0.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-02-07 16:44:02.000000 spacy-huggingface-hub-0.0.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-07 16:44:07.990889 spacy-huggingface-hub-0.0.9/spacy_huggingface_hub/
+-rw-r--r--   0 vsts      (1001) docker     (122)       37 2023-02-07 16:44:02.000000 spacy-huggingface-hub-0.0.9/spacy_huggingface_hub/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      135 2023-02-07 16:44:02.000000 spacy-huggingface-hub-0.0.9/spacy_huggingface_hub/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10801 2023-02-07 16:44:02.000000 spacy-huggingface-hub-0.0.9/spacy_huggingface_hub/push.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-07 16:44:07.990889 spacy-huggingface-hub-0.0.9/spacy_huggingface_hub.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5340 2023-02-07 16:44:07.000000 spacy-huggingface-hub-0.0.9/spacy_huggingface_hub.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      418 2023-02-07 16:44:07.000000 spacy-huggingface-hub-0.0.9/spacy_huggingface_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-02-07 16:44:07.000000 spacy-huggingface-hub-0.0.9/spacy_huggingface_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-02-07 16:44:07.000000 spacy-huggingface-hub-0.0.9/spacy_huggingface_hub.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       71 2023-02-07 16:44:07.000000 spacy-huggingface-hub-0.0.9/spacy_huggingface_hub.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       22 2023-02-07 16:44:07.000000 spacy-huggingface-hub-0.0.9/spacy_huggingface_hub.egg-info/top_level.txt
```

### Comparing `spacy-huggingface-hub-0.0.8/LICENSE` & `spacy-huggingface-hub-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-huggingface-hub-0.0.8/PKG-INFO` & `spacy-huggingface-hub-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-huggingface-hub
-Version: 0.0.8
+Version: 0.0.9
 Summary: Quickly push your spaCy pipelines to the Hugging Face Hub
 Home-page: https://spacy.io
 Author: Explosion and Hugging Face
 Author-email: omar@huggingface.co
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-huggingface-hub Version: 0.0.8 Summary:
+Metadata-Version: 2.1 Name: spacy-huggingface-hub Version: 0.0.9 Summary:
 Quickly push your spaCy pipelines to the Hugging Face Hub Home-page: https://
 spacy.io Author: Explosion and Hugging Face Author-email: omar@huggingface.co
 License: MIT Classifier: Development Status :: 4 - Beta Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
```

### Comparing `spacy-huggingface-hub-0.0.8/README.md` & `spacy-huggingface-hub-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `spacy-huggingface-hub-0.0.8/setup.cfg` & `spacy-huggingface-hub-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.8
+version = 0.0.9
 description = Quickly push your spaCy pipelines to the Hugging Face Hub
 url = https://spacy.io
 author = Explosion and Hugging Face
 author_email = omar@huggingface.co
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -17,17 +17,17 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 
 [options]
 python_requires = >=3.6
 install_requires = 
-	huggingface_hub>=0.8.1,<0.9.0
+	huggingface_hub>=0.8.1
 	wasabi>=0.8.1,<1.2.0
-	typer>=0.3.0,<0.5.0
+	typer>=0.3.0,<0.8.0
 	PyYAML
 
 [options.entry_points]
 spacy_cli = 
 	huggingface-hub = spacy_huggingface_hub.push:huggingface_hub_push_cli
 
 [flake8]
```

### Comparing `spacy-huggingface-hub-0.0.8/spacy_huggingface_hub/push.py` & `spacy-huggingface-hub-0.0.9/spacy_huggingface_hub/push.py`

 * *Files identical despite different names*

### Comparing `spacy-huggingface-hub-0.0.8/spacy_huggingface_hub.egg-info/PKG-INFO` & `spacy-huggingface-hub-0.0.9/spacy_huggingface_hub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-huggingface-hub
-Version: 0.0.8
+Version: 0.0.9
 Summary: Quickly push your spaCy pipelines to the Hugging Face Hub
 Home-page: https://spacy.io
 Author: Explosion and Hugging Face
 Author-email: omar@huggingface.co
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-huggingface-hub Version: 0.0.8 Summary:
+Metadata-Version: 2.1 Name: spacy-huggingface-hub Version: 0.0.9 Summary:
 Quickly push your spaCy pipelines to the Hugging Face Hub Home-page: https://
 spacy.io Author: Explosion and Hugging Face Author-email: omar@huggingface.co
 License: MIT Classifier: Development Status :: 4 - Beta Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
```


# Comparing `tmp/pertCF-0.1.3.tar.gz` & `tmp/pertCF-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pertCF-0.1.3.tar", last modified: Mon Jul  3 13:31:22 2023, max compression
+gzip compressed data, was "pertCF-0.1.4.tar", last modified: Mon Jul  3 13:52:16 2023, max compression
```

## Comparing `pertCF-0.1.3.tar` & `pertCF-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 13:31:22.078225 pertCF-0.1.3/
--rw-r--r--   0 bbayrak    (501) staff       (20)     1061 2023-07-03 13:13:48.000000 pertCF-0.1.3/LICENSE.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 13:31:22.078063 pertCF-0.1.3/PKG-INFO
-drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 13:31:22.076857 pertCF-0.1.3/PertCF/
--rw-r--r--   0 bbayrak    (501) staff       (20)     1015 2023-07-03 11:03:30.000000 pertCF-0.1.3/PertCF/Case.py
--rw-r--r--   0 bbayrak    (501) staff       (20)     2329 2023-07-03 10:52:27.000000 pertCF-0.1.3/PertCF/Data.py
--rw-r--r--   0 bbayrak    (501) staff       (20)     7304 2023-07-03 11:21:49.000000 pertCF-0.1.3/PertCF/PertCF.py
--rw-r--r--   0 bbayrak    (501) staff       (20)     4046 2023-07-03 10:52:27.000000 pertCF-0.1.3/PertCF/Similarity.py
--rw-r--r--   0 bbayrak    (501) staff       (20)      185 2023-07-03 13:30:03.000000 pertCF-0.1.3/PertCF/__init__.py
--rw-r--r--   0 bbayrak    (501) staff       (20)        9 2023-07-03 12:04:43.000000 pertCF-0.1.3/README.md
-drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 13:31:22.077839 pertCF-0.1.3/pertCF.egg-info/
--rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 13:31:22.000000 pertCF-0.1.3/pertCF.egg-info/PKG-INFO
--rw-r--r--   0 bbayrak    (501) staff       (20)      266 2023-07-03 13:31:22.000000 pertCF-0.1.3/pertCF.egg-info/SOURCES.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)        1 2023-07-03 13:31:22.000000 pertCF-0.1.3/pertCF.egg-info/dependency_links.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)       42 2023-07-03 13:31:22.000000 pertCF-0.1.3/pertCF.egg-info/requires.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)        7 2023-07-03 13:31:22.000000 pertCF-0.1.3/pertCF.egg-info/top_level.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)       38 2023-07-03 13:31:22.078275 pertCF-0.1.3/setup.cfg
--rw-r--r--   0 bbayrak    (501) staff       (20)      994 2023-07-03 13:30:43.000000 pertCF-0.1.3/setup.py
+drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 13:52:16.006087 pertCF-0.1.4/
+-rw-r--r--   0 bbayrak    (501) staff       (20)     1061 2023-07-03 13:13:48.000000 pertCF-0.1.4/LICENSE.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 13:52:16.005907 pertCF-0.1.4/PKG-INFO
+drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 13:52:16.004423 pertCF-0.1.4/PertCF/
+-rw-r--r--   0 bbayrak    (501) staff       (20)     1015 2023-07-03 11:03:30.000000 pertCF-0.1.4/PertCF/Case.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)     2329 2023-07-03 10:52:27.000000 pertCF-0.1.4/PertCF/Data.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)     7304 2023-07-03 11:21:49.000000 pertCF-0.1.4/PertCF/PertCF.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)     4046 2023-07-03 10:52:27.000000 pertCF-0.1.4/PertCF/Similarity.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)      161 2023-07-03 13:46:27.000000 pertCF-0.1.4/PertCF/__init__.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)        9 2023-07-03 12:04:43.000000 pertCF-0.1.4/README.md
+drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 13:52:16.005589 pertCF-0.1.4/pertCF.egg-info/
+-rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 13:52:15.000000 pertCF-0.1.4/pertCF.egg-info/PKG-INFO
+-rw-r--r--   0 bbayrak    (501) staff       (20)      266 2023-07-03 13:52:15.000000 pertCF-0.1.4/pertCF.egg-info/SOURCES.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)        1 2023-07-03 13:52:15.000000 pertCF-0.1.4/pertCF.egg-info/dependency_links.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)       42 2023-07-03 13:52:15.000000 pertCF-0.1.4/pertCF.egg-info/requires.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)        7 2023-07-03 13:52:15.000000 pertCF-0.1.4/pertCF.egg-info/top_level.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)       38 2023-07-03 13:52:16.006151 pertCF-0.1.4/setup.cfg
+-rw-r--r--   0 bbayrak    (501) staff       (20)      994 2023-07-03 13:49:25.000000 pertCF-0.1.4/setup.py
```

### Comparing `pertCF-0.1.3/LICENSE.txt` & `pertCF-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.3/PertCF/Case.py` & `pertCF-0.1.4/PertCF/Case.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.3/PertCF/Data.py` & `pertCF-0.1.4/PertCF/Data.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.3/PertCF/PertCF.py` & `pertCF-0.1.4/PertCF/PertCF.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.3/PertCF/Similarity.py` & `pertCF-0.1.4/PertCF/Similarity.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.3/setup.py` & `pertCF-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 # with open('HISTORY.md') as history_file:
 #     HISTORY = history_file.read()
 #
 setup_args = dict(
     name='pertCF',
-    version='0.1.3',
+    version='0.1.4',
     description='PertCF explainer is a counterfactual based XAI technique.',
     # long_description_content_type="text/markdown",
     # long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Betül Bayrak',
     author_email='betul.bayrak@ntnu.no',
```


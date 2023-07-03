# Comparing `tmp/pertCF-0.1.1.tar.gz` & `tmp/pertCF-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pertCF-0.1.1.tar", last modified: Mon Jul  3 12:57:40 2023, max compression
+gzip compressed data, was "pertCF-0.1.2.tar", last modified: Mon Jul  3 13:14:57 2023, max compression
```

## Comparing `pertCF-0.1.1.tar` & `pertCF-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 12:57:40.494182 pertCF-0.1.1/
--rw-r--r--   0 bbayrak    (501) staff       (20)       30 2023-07-03 12:46:12.000000 pertCF-0.1.1/LICENSE.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 12:57:40.494003 pertCF-0.1.1/PKG-INFO
-drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 12:57:40.492661 pertCF-0.1.1/PertCF/
--rw-r--r--   0 bbayrak    (501) staff       (20)     1015 2023-07-03 11:03:30.000000 pertCF-0.1.1/PertCF/Case.py
--rw-r--r--   0 bbayrak    (501) staff       (20)     2329 2023-07-03 10:52:27.000000 pertCF-0.1.1/PertCF/Data.py
--rw-r--r--   0 bbayrak    (501) staff       (20)     7304 2023-07-03 11:21:49.000000 pertCF-0.1.1/PertCF/PertCF.py
--rw-r--r--   0 bbayrak    (501) staff       (20)     4046 2023-07-03 10:52:27.000000 pertCF-0.1.1/PertCF/Similarity.py
--rw-r--r--   0 bbayrak    (501) staff       (20)      173 2023-07-03 12:29:32.000000 pertCF-0.1.1/PertCF/__init__.py
--rw-r--r--   0 bbayrak    (501) staff       (20)        9 2023-07-03 12:04:43.000000 pertCF-0.1.1/README.md
-drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 12:57:40.493776 pertCF-0.1.1/pertCF.egg-info/
--rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 12:57:40.000000 pertCF-0.1.1/pertCF.egg-info/PKG-INFO
--rw-r--r--   0 bbayrak    (501) staff       (20)      266 2023-07-03 12:57:40.000000 pertCF-0.1.1/pertCF.egg-info/SOURCES.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)        1 2023-07-03 12:57:40.000000 pertCF-0.1.1/pertCF.egg-info/dependency_links.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)       65 2023-07-03 12:57:40.000000 pertCF-0.1.1/pertCF.egg-info/requires.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)        7 2023-07-03 12:57:40.000000 pertCF-0.1.1/pertCF.egg-info/top_level.txt
--rw-r--r--   0 bbayrak    (501) staff       (20)       38 2023-07-03 12:57:40.494233 pertCF-0.1.1/setup.cfg
--rw-r--r--   0 bbayrak    (501) staff       (20)      949 2023-07-03 12:56:39.000000 pertCF-0.1.1/setup.py
+drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 13:14:57.385219 pertCF-0.1.2/
+-rw-r--r--   0 bbayrak    (501) staff       (20)     1061 2023-07-03 13:13:48.000000 pertCF-0.1.2/LICENSE.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 13:14:57.385029 pertCF-0.1.2/PKG-INFO
+drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 13:14:57.383737 pertCF-0.1.2/PertCF/
+-rw-r--r--   0 bbayrak    (501) staff       (20)     1015 2023-07-03 11:03:30.000000 pertCF-0.1.2/PertCF/Case.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)     2329 2023-07-03 10:52:27.000000 pertCF-0.1.2/PertCF/Data.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)     7304 2023-07-03 11:21:49.000000 pertCF-0.1.2/PertCF/PertCF.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)     4046 2023-07-03 10:52:27.000000 pertCF-0.1.2/PertCF/Similarity.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)      173 2023-07-03 12:29:32.000000 pertCF-0.1.2/PertCF/__init__.py
+-rw-r--r--   0 bbayrak    (501) staff       (20)        9 2023-07-03 12:04:43.000000 pertCF-0.1.2/README.md
+drwxr-xr-x   0 bbayrak    (501) staff       (20)        0 2023-07-03 13:14:57.384779 pertCF-0.1.2/pertCF.egg-info/
+-rw-r--r--   0 bbayrak    (501) staff       (20)      261 2023-07-03 13:14:57.000000 pertCF-0.1.2/pertCF.egg-info/PKG-INFO
+-rw-r--r--   0 bbayrak    (501) staff       (20)      266 2023-07-03 13:14:57.000000 pertCF-0.1.2/pertCF.egg-info/SOURCES.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)        1 2023-07-03 13:14:57.000000 pertCF-0.1.2/pertCF.egg-info/dependency_links.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)       42 2023-07-03 13:14:57.000000 pertCF-0.1.2/pertCF.egg-info/requires.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)        7 2023-07-03 13:14:57.000000 pertCF-0.1.2/pertCF.egg-info/top_level.txt
+-rw-r--r--   0 bbayrak    (501) staff       (20)       38 2023-07-03 13:14:57.385278 pertCF-0.1.2/setup.cfg
+-rw-r--r--   0 bbayrak    (501) staff       (20)      994 2023-07-03 13:14:17.000000 pertCF-0.1.2/setup.py
```

### Comparing `pertCF-0.1.1/PertCF/Case.py` & `pertCF-0.1.2/PertCF/Case.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.1/PertCF/Data.py` & `pertCF-0.1.2/PertCF/Data.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.1/PertCF/PertCF.py` & `pertCF-0.1.2/PertCF/PertCF.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.1/PertCF/Similarity.py` & `pertCF-0.1.2/PertCF/Similarity.py`

 * *Files identical despite different names*

### Comparing `pertCF-0.1.1/setup.py` & `pertCF-0.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,30 +4,33 @@
     README = readme_file.read()
 
 # with open('HISTORY.md') as history_file:
 #     HISTORY = history_file.read()
 #
 setup_args = dict(
     name='pertCF',
-    version='0.1.1',
+    version='0.1.2',
     description='PertCF explainer is a counterfactual based XAI technique.',
     # long_description_content_type="text/markdown",
     # long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Betül Bayrak',
     author_email='betul.bayrak@ntnu.no',
     keywords=['pertCF', 'XAI', 'Explanation', 'Counterfactual'],
     # url='https://github.com/ncthuc/elastictools',
     # download_url='https://pypi.org/project/elastictools/'
 )
 
 install_requires = [
-    'numpy == 1.23.5',
-    'shap == 0.41.0',
-    'pandas == 2.0.2',
+    # 'numpy <= 1.23.5',
+    # 'shap <= 0.41.0',
+    # 'pandas <= 2.0.2',
+    'numpy',
+    'shap',
+    'pandas',
     'scipy',
     'category_encoders'
 ]
 
 if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```


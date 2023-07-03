# Comparing `tmp/datawhispers-0.2.8.1.tar.gz` & `tmp/datawhispers-0.2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawhispers-0.2.8.1.tar", last modified: Sun Jul  2 18:56:43 2023, max compression
+gzip compressed data, was "datawhispers-0.2.8.2.tar", last modified: Mon Jul  3 08:48:47 2023, max compression
```

## Comparing `datawhispers-0.2.8.1.tar` & `datawhispers-0.2.8.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-02 18:56:43.737533 datawhispers-0.2.8.1/
--rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.8.1/LICENSE
--rw-r--r--   0 german     (501) staff       (20)     1816 2023-07-02 18:56:43.737401 datawhispers-0.2.8.1/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      693 2023-07-02 18:56:31.000000 datawhispers-0.2.8.1/README.md
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-02 18:56:43.736588 datawhispers-0.2.8.1/datawhispers/
--rw-r--r--   0 german     (501) staff       (20)       74 2023-07-02 18:37:43.000000 datawhispers-0.2.8.1/datawhispers/__init__.py
--rw-r--r--   0 german     (501) staff       (20)     8342 2023-07-02 11:15:25.000000 datawhispers-0.2.8.1/datawhispers/advancedProg.py
--rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-01 09:48:05.000000 datawhispers-0.2.8.1/datawhispers/datavis.py
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-02 18:56:43.737194 datawhispers-0.2.8.1/datawhispers.egg-info/
--rw-r--r--   0 german     (501) staff       (20)     1816 2023-07-02 18:56:43.000000 datawhispers-0.2.8.1/datawhispers.egg-info/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      283 2023-07-02 18:56:43.000000 datawhispers-0.2.8.1/datawhispers.egg-info/SOURCES.txt
--rw-r--r--   0 german     (501) staff       (20)        1 2023-07-02 18:56:43.000000 datawhispers-0.2.8.1/datawhispers.egg-info/dependency_links.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-02 18:56:43.000000 datawhispers-0.2.8.1/datawhispers.egg-info/requires.txt
--rw-r--r--   0 german     (501) staff       (20)       13 2023-07-02 18:56:43.000000 datawhispers-0.2.8.1/datawhispers.egg-info/top_level.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-02 18:56:43.737581 datawhispers-0.2.8.1/setup.cfg
--rw-r--r--   0 german     (501) staff       (20)     2273 2023-07-02 18:53:14.000000 datawhispers-0.2.8.1/setup.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-03 08:48:47.621478 datawhispers-0.2.8.2/
+-rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.8.2/LICENSE
+-rw-r--r--   0 german     (501) staff       (20)     1816 2023-07-03 08:48:47.621340 datawhispers-0.2.8.2/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      694 2023-07-02 18:58:56.000000 datawhispers-0.2.8.2/README.md
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-03 08:48:47.620430 datawhispers-0.2.8.2/datawhispers/
+-rw-r--r--   0 german     (501) staff       (20)      111 2023-07-03 08:22:12.000000 datawhispers-0.2.8.2/datawhispers/__init__.py
+-rw-r--r--   0 german     (501) staff       (20)     8342 2023-07-03 08:30:46.000000 datawhispers-0.2.8.2/datawhispers/advancedProg.py
+-rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-03 08:34:03.000000 datawhispers-0.2.8.2/datawhispers/datavis.py
+-rw-r--r--   0 german     (501) staff       (20)        0 2023-07-03 08:22:31.000000 datawhispers-0.2.8.2/datawhispers/mathFuncs.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-03 08:48:47.621137 datawhispers-0.2.8.2/datawhispers.egg-info/
+-rw-r--r--   0 german     (501) staff       (20)     1816 2023-07-03 08:48:47.000000 datawhispers-0.2.8.2/datawhispers.egg-info/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      309 2023-07-03 08:48:47.000000 datawhispers-0.2.8.2/datawhispers.egg-info/SOURCES.txt
+-rw-r--r--   0 german     (501) staff       (20)        1 2023-07-03 08:48:47.000000 datawhispers-0.2.8.2/datawhispers.egg-info/dependency_links.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-03 08:48:47.000000 datawhispers-0.2.8.2/datawhispers.egg-info/requires.txt
+-rw-r--r--   0 german     (501) staff       (20)       13 2023-07-03 08:48:47.000000 datawhispers-0.2.8.2/datawhispers.egg-info/top_level.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-03 08:48:47.621531 datawhispers-0.2.8.2/setup.cfg
+-rw-r--r--   0 german     (501) staff       (20)     2273 2023-07-03 08:48:18.000000 datawhispers-0.2.8.2/setup.py
```

### Comparing `datawhispers-0.2.8.1/LICENSE` & `datawhispers-0.2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.1/PKG-INFO` & `datawhispers-0.2.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.8.1
+Version: 0.2.8.2
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.8.1/README.md` & `datawhispers-0.2.8.2/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 
 ### The **DataWhispers** module is used for solving regression and statistical problems
 
 It was programmed for exams in advanced programming and data visualisation at DHBW Mannheim
 
 Solve regression problems (lin, poly, trig, free, least_squares), plot the results and mnist numbers or do some statistical analysis with chi2, pearson or student-t
 
-To install just write ```pip install datawhispers``` in your command prompt of choice
+To install just write ```pip install datawhispers``` in your command prompt of choice
```

### Comparing `datawhispers-0.2.8.1/datawhispers/advancedProg.py` & `datawhispers-0.2.8.2/datawhispers/advancedProg.py`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.1/datawhispers/datavis.py` & `datawhispers-0.2.8.2/datawhispers/datavis.py`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.8.1/datawhispers.egg-info/PKG-INFO` & `datawhispers-0.2.8.2/datawhispers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.8.1
+Version: 0.2.8.2
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.8.1/setup.py` & `datawhispers-0.2.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
   name = 'datawhispers',         # How you named your package folder (MyLib)
   packages = ["datawhispers"],   # Chose the same as "name"
-  version = '0.2.8.1',      # Start with a small number and increase it with every change you make
+  version = '0.2.8.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation',   # Give a short description about your library
   author = 'German Paul',                   # Type in your name
   author_email = 'motets-rosiest-0r@icloud.com',      # Type in your E-Mail
   url = 'https://github.com/GermanPaul12/datawhispers',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Python3', 'Data Visualisation', 'Statistical Analysis', "Regression", "Advanced Programming"],   # Keywords that define your package best
```


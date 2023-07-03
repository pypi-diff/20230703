# Comparing `tmp/pycse-2.2.3.tar.gz` & `tmp/pycse-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycse-2.2.3.tar", last modified: Mon Jun 12 12:42:28 2023, max compression
+gzip compressed data, was "pycse-2.2.4.tar", last modified: Mon Jul  3 17:15:34 2023, max compression
```

## Comparing `pycse-2.2.3.tar` & `pycse-2.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jkitchin   (501) staff       (20)        0 2023-06-12 12:42:28.422922 pycse-2.2.3/
--rw-r--r--   0 jkitchin   (501) staff       (20)    18091 2021-06-26 14:31:14.000000 pycse-2.2.3/LICENSE
--rw-r--r--   0 jkitchin   (501) staff       (20)      527 2023-06-12 12:42:28.423026 pycse-2.2.3/PKG-INFO
-drwxr-xr-x   0 jkitchin   (501) staff       (20)        0 2023-06-12 12:42:28.421047 pycse-2.2.3/pycse/
--rw-r--r--   0 jkitchin   (501) staff       (20)    10413 2023-06-11 20:54:31.000000 pycse-2.2.3/pycse/PYCSE.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     2567 2023-02-01 22:27:33.000000 pycse-2.2.3/pycse/__init__.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     5165 2023-06-11 17:37:43.000000 pycse-2.2.3/pycse/beginner.py
--rwxr-xr-x   0 jkitchin   (501) staff       (20)     3032 2023-06-12 12:37:32.000000 pycse-2.2.3/pycse/cli.py
--rw-r--r--   0 jkitchin   (501) staff       (20)    19347 2022-05-22 16:38:59.000000 pycse-2.2.3/pycse/colab.py
--rw-r--r--   0 jkitchin   (501) staff       (20)    34116 2022-04-25 17:32:11.000000 pycse-2.2.3/pycse/colors.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     6387 2023-06-11 15:24:44.000000 pycse-2.2.3/pycse/hashcache.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     6753 2022-05-22 16:38:58.000000 pycse-2.2.3/pycse/lisp.py
--rw-r--r--   0 jkitchin   (501) staff       (20)      726 2022-05-22 16:38:58.000000 pycse-2.2.3/pycse/obipython.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     6424 2022-05-22 16:38:58.000000 pycse-2.2.3/pycse/orgmode.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     6897 2022-05-22 16:38:58.000000 pycse-2.2.3/pycse/orgmode_v1.py
--rw-r--r--   0 jkitchin   (501) staff       (20)      857 2023-01-31 00:05:57.000000 pycse-2.2.3/pycse/plotly.py
--rw-r--r--   0 jkitchin   (501) staff       (20)      714 2022-04-25 23:28:56.000000 pycse-2.2.3/pycse/sandbox.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     3333 2022-07-18 13:27:29.000000 pycse-2.2.3/pycse/search.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     2136 2022-05-22 16:38:58.000000 pycse-2.2.3/pycse/utils.py
-drwxr-xr-x   0 jkitchin   (501) staff       (20)        0 2023-06-12 12:42:28.422686 pycse-2.2.3/pycse.egg-info/
--rw-r--r--   0 jkitchin   (501) staff       (20)      527 2023-06-12 12:42:28.000000 pycse-2.2.3/pycse.egg-info/PKG-INFO
--rw-r--r--   0 jkitchin   (501) staff       (20)      467 2023-06-12 12:42:28.000000 pycse-2.2.3/pycse.egg-info/SOURCES.txt
--rw-r--r--   0 jkitchin   (501) staff       (20)        1 2023-06-12 12:42:28.000000 pycse-2.2.3/pycse.egg-info/dependency_links.txt
--rw-r--r--   0 jkitchin   (501) staff       (20)       42 2023-06-12 12:42:28.000000 pycse-2.2.3/pycse.egg-info/entry_points.txt
--rw-r--r--   0 jkitchin   (501) staff       (20)       25 2023-06-12 12:42:28.000000 pycse-2.2.3/pycse.egg-info/requires.txt
--rw-r--r--   0 jkitchin   (501) staff       (20)        6 2023-06-12 12:42:28.000000 pycse-2.2.3/pycse.egg-info/top_level.txt
--rw-r--r--   0 jkitchin   (501) staff       (20)       27 2023-06-11 15:25:22.000000 pycse-2.2.3/requirements.txt
--rw-r--r--   0 jkitchin   (501) staff       (20)      271 2023-06-12 12:42:28.423463 pycse-2.2.3/setup.cfg
--rw-r--r--   0 jkitchin   (501) staff       (20)     1187 2023-06-12 12:40:06.000000 pycse-2.2.3/setup.py
+drwxr-xr-x   0 jkitchin   (501) staff       (20)        0 2023-07-03 17:15:34.813187 pycse-2.2.4/
+-rw-r--r--   0 jkitchin   (501) staff       (20)    18091 2021-06-26 14:31:14.000000 pycse-2.2.4/LICENSE
+-rw-r--r--   0 jkitchin   (501) staff       (20)      527 2023-07-03 17:15:34.813301 pycse-2.2.4/PKG-INFO
+drwxr-xr-x   0 jkitchin   (501) staff       (20)        0 2023-07-03 17:15:34.811131 pycse-2.2.4/pycse/
+-rw-r--r--   0 jkitchin   (501) staff       (20)    10413 2023-06-11 20:54:31.000000 pycse-2.2.4/pycse/PYCSE.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     2567 2023-02-01 22:27:33.000000 pycse-2.2.4/pycse/__init__.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     5165 2023-06-11 17:37:43.000000 pycse-2.2.4/pycse/beginner.py
+-rwxr--r--   0 jkitchin   (501) staff       (20)     3217 2023-06-16 12:45:31.000000 pycse-2.2.4/pycse/cli.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)    19347 2022-05-22 16:38:59.000000 pycse-2.2.4/pycse/colab.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)    34116 2022-04-25 17:32:11.000000 pycse-2.2.4/pycse/colors.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     6387 2023-06-11 15:24:44.000000 pycse-2.2.4/pycse/hashcache.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     6753 2022-05-22 16:38:58.000000 pycse-2.2.4/pycse/lisp.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)      726 2022-05-22 16:38:58.000000 pycse-2.2.4/pycse/obipython.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     6424 2022-05-22 16:38:58.000000 pycse-2.2.4/pycse/orgmode.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     6897 2022-05-22 16:38:58.000000 pycse-2.2.4/pycse/orgmode_v1.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)      857 2023-01-31 00:05:57.000000 pycse-2.2.4/pycse/plotly.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)      714 2022-04-25 23:28:56.000000 pycse-2.2.4/pycse/sandbox.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     3333 2022-07-18 13:27:29.000000 pycse-2.2.4/pycse/search.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     2136 2022-05-22 16:38:58.000000 pycse-2.2.4/pycse/utils.py
+drwxr-xr-x   0 jkitchin   (501) staff       (20)        0 2023-07-03 17:15:34.812939 pycse-2.2.4/pycse.egg-info/
+-rw-r--r--   0 jkitchin   (501) staff       (20)      527 2023-07-03 17:15:34.000000 pycse-2.2.4/pycse.egg-info/PKG-INFO
+-rw-r--r--   0 jkitchin   (501) staff       (20)      467 2023-07-03 17:15:34.000000 pycse-2.2.4/pycse.egg-info/SOURCES.txt
+-rw-r--r--   0 jkitchin   (501) staff       (20)        1 2023-07-03 17:15:34.000000 pycse-2.2.4/pycse.egg-info/dependency_links.txt
+-rw-r--r--   0 jkitchin   (501) staff       (20)       42 2023-07-03 17:15:34.000000 pycse-2.2.4/pycse.egg-info/entry_points.txt
+-rw-r--r--   0 jkitchin   (501) staff       (20)       50 2023-07-03 17:15:34.000000 pycse-2.2.4/pycse.egg-info/requires.txt
+-rw-r--r--   0 jkitchin   (501) staff       (20)        6 2023-07-03 17:15:34.000000 pycse-2.2.4/pycse.egg-info/top_level.txt
+-rw-r--r--   0 jkitchin   (501) staff       (20)       45 2023-07-03 17:14:49.000000 pycse-2.2.4/requirements.txt
+-rw-r--r--   0 jkitchin   (501) staff       (20)      313 2023-07-03 17:15:34.813776 pycse-2.2.4/setup.cfg
+-rw-r--r--   0 jkitchin   (501) staff       (20)     1276 2023-07-03 17:14:57.000000 pycse-2.2.4/setup.py
```

### Comparing `pycse-2.2.3/LICENSE` & `pycse-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/PKG-INFO` & `pycse-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycse
-Version: 2.2.3
+Version: 2.2.4
 Summary: python computations in science and engineering
 Home-page: https://github.com/jkitchin/pycse
 Maintainer: John Kitchin
 Maintainer-email: jkitchin@andrew.cmu.edu
 License: GPL
 Platform: linux
 License-File: LICENSE
```

### Comparing `pycse-2.2.3/pycse/PYCSE.py` & `pycse-2.2.4/pycse/PYCSE.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/__init__.py` & `pycse-2.2.4/pycse/__init__.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/beginner.py` & `pycse-2.2.4/pycse/beginner.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/cli.py` & `pycse-2.2.4/pycse/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 
 
 Sometimes you have to manually delete an old container if it doesn't close
 properly. This should do it:
 
 > docker rm -f pycse
 
+The Docker Desktop app is also helpful for this kind of stuff.
+
+TODO: make this a click app, with cli arguments to update the image? e.g.
+
+> pycse --update
+> pycse path/to/working-dir
+
 """
 
 import os
 import uuid
 import numpy as np
 import time
 import webbrowser
```

### Comparing `pycse-2.2.3/pycse/colab.py` & `pycse-2.2.4/pycse/colab.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/colors.py` & `pycse-2.2.4/pycse/colors.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/hashcache.py` & `pycse-2.2.4/pycse/hashcache.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/lisp.py` & `pycse-2.2.4/pycse/lisp.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/obipython.py` & `pycse-2.2.4/pycse/obipython.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/orgmode.py` & `pycse-2.2.4/pycse/orgmode.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/orgmode_v1.py` & `pycse-2.2.4/pycse/orgmode_v1.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/plotly.py` & `pycse-2.2.4/pycse/plotly.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/sandbox.py` & `pycse-2.2.4/pycse/sandbox.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/search.py` & `pycse-2.2.4/pycse/search.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse/utils.py` & `pycse-2.2.4/pycse/utils.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.3/pycse.egg-info/PKG-INFO` & `pycse-2.2.4/pycse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycse
-Version: 2.2.3
+Version: 2.2.4
 Summary: python computations in science and engineering
 Home-page: https://github.com/jkitchin/pycse
 Maintainer: John Kitchin
 Maintainer-email: jkitchin@andrew.cmu.edu
 License: GPL
 Platform: linux
 License-File: LICENSE
```

### Comparing `pycse-2.2.3/setup.py` & `pycse-2.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 # Copyright 2015-2021 John Kitchin
 # (see accompanying license files for details).
 from setuptools import setup
 
 setup(
     name="pycse",
-    version="2.2.3",
+    version="2.2.4",
     description="python computations in science and engineering",
     url="https://github.com/jkitchin/pycse",
     maintainer="John Kitchin",
     maintainer_email="jkitchin@andrew.cmu.edu",
     license="GPL",
     platforms=["linux"],
     packages=["pycse"],
     setup_requires=["nose>=1.0"],
     data_files=["requirements.txt", "LICENSE"],
-    install_requires=["numpy", "scipy", "numdifftools"],
+    install_requires=[
+        "numpy",
+        "scipy",
+        "numdifftools",
+        "pandas",
+        "joblib",
+        "matplotlib",
+    ],
     entry_points={"console_scripts": ["pycse = pycse.cli:pycse"]},
     long_description="""\
 python computations in science and engineering
 ===============================================
 
 This package provides functions that are useful in science and engineering
 computations.
```


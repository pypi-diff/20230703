# Comparing `tmp/mathkit-1.1.0.tar.gz` & `tmp/mathkit-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathkit-1.1.0.tar", last modified: Sun Jul  2 04:56:38 2023, max compression
+gzip compressed data, was "mathkit-1.1.1.tar", last modified: Mon Jul  3 06:18:23 2023, max compression
```

## Comparing `mathkit-1.1.0.tar` & `mathkit-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 04:56:38.678902 mathkit-1.1.0/
--rw-rw-rw-   0        0        0     3466 2023-07-02 04:56:38.677895 mathkit-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3021 2023-07-02 02:47:56.000000 mathkit-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 04:56:38.658580 mathkit-1.1.0/mathkit/
--rw-rw-rw-   0        0        0      513 2023-07-02 03:44:28.000000 mathkit-1.1.0/mathkit/__init__.py
--rw-rw-rw-   0        0        0     9800 2023-07-02 04:56:06.000000 mathkit-1.1.0/mathkit/main.py
-drwxrwxrwx   0        0        0        0 2023-07-02 04:56:38.674354 mathkit-1.1.0/mathkit.egg-info/
--rw-rw-rw-   0        0        0     3466 2023-07-02 04:56:38.000000 mathkit-1.1.0/mathkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-07-02 04:56:38.000000 mathkit-1.1.0/mathkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 04:56:38.000000 mathkit-1.1.0/mathkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-02 04:56:38.000000 mathkit-1.1.0/mathkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 04:56:38.678902 mathkit-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      712 2023-07-02 04:56:32.000000 mathkit-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:18:23.492493 mathkit-1.1.1/
+-rw-rw-rw-   0        0        0     3466 2023-07-03 06:18:23.474308 mathkit-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3021 2023-07-02 02:47:56.000000 mathkit-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 06:18:23.381145 mathkit-1.1.1/mathkit/
+-rw-rw-rw-   0        0        0      527 2023-07-03 06:17:43.000000 mathkit-1.1.1/mathkit/__init__.py
+-rw-rw-rw-   0        0        0     9800 2023-07-02 04:56:06.000000 mathkit-1.1.1/mathkit/main.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:18:23.463141 mathkit-1.1.1/mathkit.egg-info/
+-rw-rw-rw-   0        0        0     3466 2023-07-03 06:18:23.000000 mathkit-1.1.1/mathkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-07-03 06:18:23.000000 mathkit-1.1.1/mathkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 06:18:23.000000 mathkit-1.1.1/mathkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 06:18:23.000000 mathkit-1.1.1/mathkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 06:18:23.494323 mathkit-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      712 2023-07-03 06:18:19.000000 mathkit-1.1.1/setup.py
```

### Comparing `mathkit-1.1.0/PKG-INFO` & `mathkit-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: TheUnkownHacker
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathkit-1.1.0/README.md` & `mathkit-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mathkit-1.1.0/mathkit/__init__.py` & `mathkit-1.1.1/mathkit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from .main import div
 from .main import fact
 from .main import hcf
 from .main import lcm
 from .main import log
 from .main import mod
 from .main import mul
-from .main import per
+from .main import percentage
 from .main import power
 from .main import sqrt
 from .main import sqr
 from .main import sub
 from .main import trig
 
-__all__ = ['add', 'cube', 'cbrt', 'div', 'fact', 'hcf', 'lcm', 'log', 'mod', 'mul', 'per', 'power', 'sqrt', 'sqr', 'sub','trig']
+__all__ = ['add', 'cube', 'cbrt', 'div', 'fact', 'hcf', 'lcm', 'log', 'mod', 'mul', 'percentage', 'power', 'sqrt', 'sqr', 'sub','trig']
```

### Comparing `mathkit-1.1.0/mathkit/main.py` & `mathkit-1.1.1/mathkit/main.py`

 * *Files identical despite different names*

### Comparing `mathkit-1.1.0/mathkit.egg-info/PKG-INFO` & `mathkit-1.1.1/mathkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: TheUnkownHacker
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathkit-1.1.0/setup.py` & `mathkit-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mathkit",
-    version="1.1.0",
+    version="1.1.1",
     author="TheUnkownHacker",
     author_email="theunkownhacker@gmail.com",
     description="Python library for mathematical functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/theunkownhacker/mathkit",
     packages=find_packages(),
```


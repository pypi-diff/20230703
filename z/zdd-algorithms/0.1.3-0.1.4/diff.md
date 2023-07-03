# Comparing `tmp/zdd_algorithms-0.1.3.tar.gz` & `tmp/zdd_algorithms-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zdd_algorithms-0.1.3.tar", last modified: Fri Jun 30 21:56:12 2023, max compression
+gzip compressed data, was "zdd_algorithms-0.1.4.tar", last modified: Mon Jul  3 08:45:32 2023, max compression
```

## Comparing `zdd_algorithms-0.1.3.tar` & `zdd_algorithms-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 21:56:12.153045 zdd_algorithms-0.1.3/
--rw-rw-rw-   0        0        0     3874 2023-06-30 21:56:12.152046 zdd_algorithms-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2581 2023-06-30 21:55:52.000000 zdd_algorithms-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 21:56:12.153045 zdd_algorithms-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1678 2023-06-30 21:56:06.000000 zdd_algorithms-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 21:56:12.135045 zdd_algorithms-0.1.3/zdd_algorithms/
--rw-rw-rw-   0        0        0      528 2023-06-30 19:18:12.000000 zdd_algorithms-0.1.3/zdd_algorithms/__init__.py
--rw-rw-rw-   0        0        0     9712 2023-06-30 19:08:05.000000 zdd_algorithms-0.1.3/zdd_algorithms/zdd.py
-drwxrwxrwx   0        0        0        0 2023-06-30 21:56:12.151046 zdd_algorithms-0.1.3/zdd_algorithms.egg-info/
--rw-rw-rw-   0        0        0     3874 2023-06-30 21:56:12.000000 zdd_algorithms-0.1.3/zdd_algorithms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-06-30 21:56:12.000000 zdd_algorithms-0.1.3/zdd_algorithms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 21:56:12.000000 zdd_algorithms-0.1.3/zdd_algorithms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-30 21:56:12.000000 zdd_algorithms-0.1.3/zdd_algorithms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-30 21:56:12.000000 zdd_algorithms-0.1.3/zdd_algorithms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 08:45:32.671157 zdd_algorithms-0.1.4/
+-rw-rw-rw-   0        0        0     3923 2023-07-03 08:45:32.670156 zdd_algorithms-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2615 2023-07-03 08:39:35.000000 zdd_algorithms-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 08:45:32.671157 zdd_algorithms-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1693 2023-07-03 08:44:44.000000 zdd_algorithms-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:45:32.651156 zdd_algorithms-0.1.4/zdd_algorithms/
+-rw-rw-rw-   0        0        0      528 2023-06-30 19:18:12.000000 zdd_algorithms-0.1.4/zdd_algorithms/__init__.py
+-rw-rw-rw-   0        0        0     9712 2023-06-30 19:08:05.000000 zdd_algorithms-0.1.4/zdd_algorithms/zdd.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:45:32.668156 zdd_algorithms-0.1.4/zdd_algorithms.egg-info/
+-rw-rw-rw-   0        0        0     3923 2023-07-03 08:45:32.000000 zdd_algorithms-0.1.4/zdd_algorithms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-07-03 08:45:32.000000 zdd_algorithms-0.1.4/zdd_algorithms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 08:45:32.000000 zdd_algorithms-0.1.4/zdd_algorithms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 08:45:32.000000 zdd_algorithms-0.1.4/zdd_algorithms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-03 08:45:32.000000 zdd_algorithms-0.1.4/zdd_algorithms.egg-info/top_level.txt
```

### Comparing `zdd_algorithms-0.1.3/PKG-INFO` & `zdd_algorithms-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: zdd_algorithms
-Version: 0.1.3
-Summary: A package that implements zdd algorithms
+Version: 0.1.4
+Summary: Implements the zdd algorithms that are on the wiki page
 Home-page: https://github.com/Thilo-J/zdd_algorithms
 Author: Thilo Langensteiner
 Author-email: <thilo.j.la@gmail.com>
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/Thilo-J/zdd_algorithms
 Description: # Zdd Algorithms
         
         Zdd algorithms is a Python library that implements the zdd algorithms that are described on the [wikipedia page](https://en.wikipedia.org/wiki/Zero-suppressed_decision_diagram). With some additional functions for creating a zdd from a set, a set from a zdd and a function to create an image of the zdd.
         
         ## Installation
         
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install zdd_wiki_algorithms.
+        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install zdd_algorithms.
         
         ```bash
-        pip install zdd_algorithms
+        pip install zdd-algorithms
         ```
         
         ## Zero-suppressed decision diagram
         
         Zdd are a special kind of binary decision diagram that represents a set of sets.
         
         <p align="center">
@@ -57,15 +57,15 @@
             frozenset({1,2})
         }
         zdd2 = zdd.to_zdd(set2)
         
         # Create an union of two zdds
         union = zdd.union(zdd1, zdd2)
         
-        # Create .PNG image of the zdd
+        # Create .PNG image of the zdd. This needs graphviz to be installed! 
         zdd.create_image(union)
         ```
         
         <p align="center">
           <img src="https://raw.githubusercontent.com/Thilo-J/zdd_algorithms/e4185fbbc28a4c59e93c847044b9b9964523dd19/13_23_12.png" alt="zdd"/>
         </p>
```

### Comparing `zdd_algorithms-0.1.3/README.md` & `zdd_algorithms-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Zdd Algorithms
 
 Zdd algorithms is a Python library that implements the zdd algorithms that are described on the [wikipedia page](https://en.wikipedia.org/wiki/Zero-suppressed_decision_diagram). With some additional functions for creating a zdd from a set, a set from a zdd and a function to create an image of the zdd.
 
 ## Installation
 
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install zdd_wiki_algorithms.
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install zdd_algorithms.
 
 ```bash
-pip install zdd_algorithms
+pip install zdd-algorithms
 ```
 
 ## Zero-suppressed decision diagram
 
 Zdd are a special kind of binary decision diagram that represents a set of sets.
 
 <p align="center">
@@ -48,15 +48,15 @@
     frozenset({1,2})
 }
 zdd2 = zdd.to_zdd(set2)
 
 # Create an union of two zdds
 union = zdd.union(zdd1, zdd2)
 
-# Create .PNG image of the zdd
+# Create .PNG image of the zdd. This needs graphviz to be installed! 
 zdd.create_image(union)
 ```
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/Thilo-J/zdd_algorithms/e4185fbbc28a4c59e93c847044b9b9964523dd19/13_23_12.png" alt="zdd"/>
 </p>
```

### Comparing `zdd_algorithms-0.1.3/setup.py` & `zdd_algorithms-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.3'
-DESCRIPTION = 'A package that implements zdd algorithms'
+VERSION = '0.1.4'
+DESCRIPTION = 'Implements the zdd algorithms that are on the wiki page'
 LONG_DESCRIPTION = 'This package implements all the algorithms described on the wiki page of zdds+\
         (union, intersection, difference, subset0, subset1, change and count). +\
         They are not optimized and without caching. This package should be used to learn zdds and +\
         play around with them. In addition to the algorithms there is also a visualization function and functions +\
         that can make a zdd out of a set and vice versa.'
```

### Comparing `zdd_algorithms-0.1.3/zdd_algorithms/__init__.py` & `zdd_algorithms-0.1.4/zdd_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `zdd_algorithms-0.1.3/zdd_algorithms/zdd.py` & `zdd_algorithms-0.1.4/zdd_algorithms/zdd.py`

 * *Files identical despite different names*

### Comparing `zdd_algorithms-0.1.3/zdd_algorithms.egg-info/PKG-INFO` & `zdd_algorithms-0.1.4/zdd_algorithms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: zdd-algorithms
-Version: 0.1.3
-Summary: A package that implements zdd algorithms
+Version: 0.1.4
+Summary: Implements the zdd algorithms that are on the wiki page
 Home-page: https://github.com/Thilo-J/zdd_algorithms
 Author: Thilo Langensteiner
 Author-email: <thilo.j.la@gmail.com>
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/Thilo-J/zdd_algorithms
 Description: # Zdd Algorithms
         
         Zdd algorithms is a Python library that implements the zdd algorithms that are described on the [wikipedia page](https://en.wikipedia.org/wiki/Zero-suppressed_decision_diagram). With some additional functions for creating a zdd from a set, a set from a zdd and a function to create an image of the zdd.
         
         ## Installation
         
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install zdd_wiki_algorithms.
+        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install zdd_algorithms.
         
         ```bash
-        pip install zdd_algorithms
+        pip install zdd-algorithms
         ```
         
         ## Zero-suppressed decision diagram
         
         Zdd are a special kind of binary decision diagram that represents a set of sets.
         
         <p align="center">
@@ -57,15 +57,15 @@
             frozenset({1,2})
         }
         zdd2 = zdd.to_zdd(set2)
         
         # Create an union of two zdds
         union = zdd.union(zdd1, zdd2)
         
-        # Create .PNG image of the zdd
+        # Create .PNG image of the zdd. This needs graphviz to be installed! 
         zdd.create_image(union)
         ```
         
         <p align="center">
           <img src="https://raw.githubusercontent.com/Thilo-J/zdd_algorithms/e4185fbbc28a4c59e93c847044b9b9964523dd19/13_23_12.png" alt="zdd"/>
         </p>
```


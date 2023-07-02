# Comparing `tmp/hyperelastic-0.1.0.tar.gz` & `tmp/hyperelastic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperelastic-0.1.0.tar", last modified: Sun Jul  2 22:18:54 2023, max compression
+gzip compressed data, was "hyperelastic-0.1.1.tar", last modified: Sun Jul  2 22:30:41 2023, max compression
```

## Comparing `hyperelastic-0.1.0.tar` & `hyperelastic-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    48636 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.819358 hyperelastic-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.823358 hyperelastic-0.1.0/src/hyperelastic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.823358 hyperelastic-0.1.0/src/hyperelastic/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/frameworks/_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/frameworks/_stretches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.823358 hyperelastic-0.1.0/src/hyperelastic/math/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/math/_voigt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.823358 hyperelastic-0.1.0/src/hyperelastic/models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/src/hyperelastic/models/invariants/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/models/invariants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/models/invariants/_third_order_deformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/src/hyperelastic/models/stretches/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/models/stretches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/models/stretches/_ogden.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/src/hyperelastic/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/spaces/_deformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/spaces/_dilatational.py
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/spaces/_distortional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.823358 hyperelastic-0.1.0/src/hyperelastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48636 2023-07-02 22:18:54.000000 hyperelastic-0.1.0/src/hyperelastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-02 22:18:54.000000 hyperelastic-0.1.0/src/hyperelastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:18:54.000000 hyperelastic-0.1.0/src/hyperelastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-02 22:18:54.000000 hyperelastic-0.1.0/src/hyperelastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 22:18:54.000000 hyperelastic-0.1.0/src/hyperelastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/tests/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/tests/test_sympy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.555144 hyperelastic-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    48635 2023-07-02 22:30:41.555144 hyperelastic-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 22:30:41.555144 hyperelastic-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.543144 hyperelastic-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.547144 hyperelastic-0.1.1/src/hyperelastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/src/hyperelastic/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/frameworks/_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/frameworks/_stretches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/src/hyperelastic/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/math/_voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/src/hyperelastic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/src/hyperelastic/models/invariants/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/models/invariants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/models/invariants/_third_order_deformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/src/hyperelastic/models/stretches/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/models/stretches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/models/stretches/_ogden.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/src/hyperelastic/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/spaces/_deformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/spaces/_dilatational.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/src/hyperelastic/spaces/_distortional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.547144 hyperelastic-0.1.1/src/hyperelastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48635 2023-07-02 22:30:41.000000 hyperelastic-0.1.1/src/hyperelastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-02 22:30:41.000000 hyperelastic-0.1.1/src/hyperelastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:30:41.000000 hyperelastic-0.1.1/src/hyperelastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-02 22:30:41.000000 hyperelastic-0.1.1/src/hyperelastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 22:30:41.000000 hyperelastic-0.1.1/src/hyperelastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:30:41.551144 hyperelastic-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/tests/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-02 22:30:32.000000 hyperelastic-0.1.1/tests/test_sympy.py
```

### Comparing `hyperelastic-0.1.0/LICENSE` & `hyperelastic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.0/PKG-INFO` & `hyperelastic-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -675,15 +675,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://felupe.readthedocs.io/en/latest
+Project-URL: Homepage, https://github.com/adtzlr/hyperelastic
 Project-URL: Code, https://github.com/adtzlr/hyperelastic
 Project-URL: Issues, https://github.com/adtzlr/hyperelastic/issues
 Keywords: python,constitution,scientific-computing,fem,finite-elements-analysis,hyperelasticity
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `hyperelastic-0.1.0/README.md` & `hyperelastic-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.0/pyproject.toml` & `hyperelastic-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -51,10 +51,10 @@
     "sympy",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "hyperelastic.__about__.__version__"}
 
 [project.urls]
-Homepage = "https://felupe.readthedocs.io/en/latest"
+Homepage = "https://github.com/adtzlr/hyperelastic"
 Code = "https://github.com/adtzlr/hyperelastic"
 Issues = "https://github.com/adtzlr/hyperelastic/issues"
```

### Comparing `hyperelastic-0.1.0/src/hyperelastic/frameworks/_invariants.py` & `hyperelastic-0.1.1/src/hyperelastic/frameworks/_invariants.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.0/src/hyperelastic/frameworks/_stretches.py` & `hyperelastic-0.1.1/src/hyperelastic/frameworks/_stretches.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.0/src/hyperelastic/math/_voigt.py` & `hyperelastic-0.1.1/src/hyperelastic/math/_voigt.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.0/src/hyperelastic/models/invariants/_third_order_deformation.py` & `hyperelastic-0.1.1/src/hyperelastic/models/invariants/_third_order_deformation.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.0/src/hyperelastic/spaces/_deformation.py` & `hyperelastic-0.1.1/src/hyperelastic/spaces/_deformation.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.0/src/hyperelastic/spaces/_dilatational.py` & `hyperelastic-0.1.1/src/hyperelastic/spaces/_dilatational.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.0/src/hyperelastic/spaces/_distortional.py` & `hyperelastic-0.1.1/src/hyperelastic/spaces/_distortional.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.0/src/hyperelastic.egg-info/PKG-INFO` & `hyperelastic-0.1.1/src/hyperelastic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -675,15 +675,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://felupe.readthedocs.io/en/latest
+Project-URL: Homepage, https://github.com/adtzlr/hyperelastic
 Project-URL: Code, https://github.com/adtzlr/hyperelastic
 Project-URL: Issues, https://github.com/adtzlr/hyperelastic/issues
 Keywords: python,constitution,scientific-computing,fem,finite-elements-analysis,hyperelasticity
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `hyperelastic-0.1.0/src/hyperelastic.egg-info/SOURCES.txt` & `hyperelastic-0.1.1/src/hyperelastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.0/tests/test_space.py` & `hyperelastic-0.1.1/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.1.0/tests/test_sympy.py` & `hyperelastic-0.1.1/tests/test_sympy.py`

 * *Files identical despite different names*


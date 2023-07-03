# Comparing `tmp/kasutils-0.0.1.tar.gz` & `tmp/kasutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kasutils-0.0.1.tar", max compression
+gzip compressed data, was "kasutils-0.0.2.tar", max compression
```

## Comparing `kasutils-0.0.1.tar` & `kasutils-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-06-27 00:59:08.786464 kasutils-0.0.1/LICENSE
--rw-r--r--   0        0        0     2168 2023-06-27 00:59:08.786464 kasutils-0.0.1/README.md
--rw-r--r--   0        0        0    14086 2023-06-27 00:59:08.786464 kasutils-0.0.1/kasutils.py
--rw-r--r--   0        0        0      546 2023-06-27 00:59:08.786464 kasutils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2774 1970-01-01 00:00:00.000000 kasutils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-03 12:41:54.474893 kasutils-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2168 2023-07-03 12:41:54.474893 kasutils-0.0.2/README.md
+-rw-r--r--   0        0        0    14068 2023-07-03 12:41:54.474893 kasutils-0.0.2/kasutils.py
+-rw-r--r--   0        0        0      546 2023-07-03 12:41:54.474893 kasutils-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2774 1970-01-01 00:00:00.000000 kasutils-0.0.2/PKG-INFO
```

### Comparing `kasutils-0.0.1/LICENSE` & `kasutils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kasutils-0.0.1/README.md` & `kasutils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kasutils-0.0.1/kasutils.py` & `kasutils-0.0.2/kasutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,8 +515,7 @@
     Geneated markdown with function name and docstring
     """
     docstrings = get_docstrings()
     for name, docstring in docstrings.items():
         docstring = docstring.replace("\n", "")
         print(f"{'#'*head_level} {name}\n - ***{docstring}***")
 
-generate_readme()
```

### Comparing `kasutils-0.0.1/pyproject.toml` & `kasutils-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=58.0.4",
     "wheel>=0.37.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "kasutils"
-version = "0.0.1"
+version = "0.0.2"
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/KasRoudra2/kasutils/"
 include = ["README.md", "LICENSE", "kasutils.py"]
 description = "My utility library with zero dependency"
 authors = ["KasRoudra <kasroudrakrd@gmail.com>"]
```

### Comparing `kasutils-0.0.1/PKG-INFO` & `kasutils-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kasutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: My utility library with zero dependency
 Home-page: https://github.com/KasRoudra2/kasutils/
 License: MIT
 Author: KasRoudra
 Author-email: kasroudrakrd@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


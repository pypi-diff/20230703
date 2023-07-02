# Comparing `tmp/sbux-0.4.0.tar.gz` & `tmp/sbux-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbux-0.4.0.tar", max compression
+gzip compressed data, was "sbux-0.4.1.tar", max compression
```

## Comparing `sbux-0.4.0.tar` & `sbux-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-06-13 13:43:20.647751 sbux-0.4.0/LICENSE
--rw-r--r--   0        0        0      907 2023-06-13 13:43:20.647751 sbux-0.4.0/README.md
--rw-r--r--   0        0        0     1136 2023-06-13 13:44:01.416388 sbux-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      153 2023-06-13 13:44:01.400388 sbux-0.4.0/src/sbux/__init__.py
--rw-r--r--   0        0        0     1686 2023-06-13 13:43:20.647751 sbux-0.4.0/src/sbux/main.py
--rw-r--r--   0        0        0      210 2023-06-13 13:43:20.647751 sbux-0.4.0/src/sbux/models/__init__.py
--rw-r--r--   0        0        0      581 2023-06-13 13:43:20.647751 sbux-0.4.0/src/sbux/models/base.py
--rw-r--r--   0        0        0     2279 2023-06-13 13:43:20.647751 sbux-0.4.0/src/sbux/models/item.py
--rw-r--r--   0        0        0     1199 2023-06-13 13:43:20.647751 sbux-0.4.0/src/sbux/models/store.py
--rw-r--r--   0        0        0     1763 1970-01-01 00:00:00.000000 sbux-0.4.0/setup.py
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 sbux-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-02 22:52:45.750326 sbux-0.4.1/LICENSE
+-rw-r--r--   0        0        0      790 2023-07-02 22:52:45.750326 sbux-0.4.1/README.md
+-rw-r--r--   0        0        0     1125 2023-07-02 22:53:15.258707 sbux-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-07-02 22:53:15.238707 sbux-0.4.1/src/sbux/__init__.py
+-rw-r--r--   0        0        0     1686 2023-07-02 22:52:45.750326 sbux-0.4.1/src/sbux/main.py
+-rw-r--r--   0        0        0      210 2023-07-02 22:52:45.750326 sbux-0.4.1/src/sbux/models/__init__.py
+-rw-r--r--   0        0        0      581 2023-07-02 22:52:45.750326 sbux-0.4.1/src/sbux/models/base.py
+-rw-r--r--   0        0        0     2279 2023-07-02 22:52:45.750326 sbux-0.4.1/src/sbux/models/item.py
+-rw-r--r--   0        0        0     1199 2023-07-02 22:52:45.750326 sbux-0.4.1/src/sbux/models/store.py
+-rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 sbux-0.4.1/PKG-INFO
```

### Comparing `sbux-0.4.0/LICENSE` & `sbux-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sbux-0.4.0/README.md` & `sbux-0.4.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # sbux
 
 [![CI](https://github.com/ngshiheng/sbux/actions/workflows/ci.yml/badge.svg)](https://github.com/ngshiheng/sbux/actions/workflows/ci.yml)
 [![Semantic Release](https://github.com/ngshiheng/sbux/actions/workflows/release.yml/badge.svg)](https://github.com/ngshiheng/sbux/actions/workflows/release.yml)
 
-`sbux` is an unofficial Starbucks Singapore (SG) software development kit (SDK).
-
-`sbux` is named after the ticker symbol of Starbucks Corporation (SBUX) on the NASDAQ.
+`sbux` is an unofficial Starbucks Singapore (SG) Python SDK.
 
 ## Installing
 
 Install and update using `pip`;
 
 ```sh
 pip install sbux
 ```
 
-## A Simple Example
+## Example
 
 ```python
 from sbux import Starbucks
 
 
 starbucks = Starbucks
 starbucks.get_stores()
```

### Comparing `sbux-0.4.0/pyproject.toml` & `sbux-0.4.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 license = "MIT"
 name = "sbux"
 packages = [
   {include = "sbux", from = "src"},
 ]
 readme = "README.md"
 repository = "https://github.com/ngshiheng/sbux"
-version = "0.4.0"
+version = "0.4.1"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "^2.28.1"
-dataclasses-json = "^0.5.7"
-requests-cache = "^1.0.1"
+requests = "2.31.0"
+dataclasses-json = "0.5.9"
+requests-cache = "1.1.0"
 
 [tool.poetry.group.dev.dependencies]
-autopep8 = "^2.0.1"
-black = "^22.12.0"
-flake8 = "^6.0.0"
-isort = "^5.11.4"
-pre-commit = "^2.21.0"
-python-semantic-release = "^7.32.2"
+autopep8 = "2.0.2"
+black = "23.3.0"
+flake8 = "6.0.0"
+isort = "5.12.0"
+pre-commit = "3.3.3"
+python-semantic-release = "7.34.6"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 extra_standard_library = ["toml"]
 line_length = 100
```

### Comparing `sbux-0.4.0/src/sbux/main.py` & `sbux-0.4.1/src/sbux/main.py`

 * *Files identical despite different names*

### Comparing `sbux-0.4.0/src/sbux/models/base.py` & `sbux-0.4.1/src/sbux/models/base.py`

 * *Files identical despite different names*

### Comparing `sbux-0.4.0/src/sbux/models/item.py` & `sbux-0.4.1/src/sbux/models/item.py`

 * *Files identical despite different names*

### Comparing `sbux-0.4.0/src/sbux/models/store.py` & `sbux-0.4.1/src/sbux/models/store.py`

 * *Files identical despite different names*

### Comparing `sbux-0.4.0/PKG-INFO` & `sbux-0.4.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 Metadata-Version: 2.1
 Name: sbux
-Version: 0.4.0
+Version: 0.4.1
 Summary: An unofficial Starbucks Singapore (SG) software development kit (SDK).
 Home-page: https://github.com/ngshiheng/sbux
 License: MIT
 Author: Jerry Ng
 Author-email: ngshiheng@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
+Requires-Dist: dataclasses-json (==0.5.9)
+Requires-Dist: requests (==2.31.0)
+Requires-Dist: requests-cache (==1.1.0)
 Project-URL: Repository, https://github.com/ngshiheng/sbux
 Description-Content-Type: text/markdown
 
 # sbux
 
 [![CI](https://github.com/ngshiheng/sbux/actions/workflows/ci.yml/badge.svg)](https://github.com/ngshiheng/sbux/actions/workflows/ci.yml)
 [![Semantic Release](https://github.com/ngshiheng/sbux/actions/workflows/release.yml/badge.svg)](https://github.com/ngshiheng/sbux/actions/workflows/release.yml)
 
-`sbux` is an unofficial Starbucks Singapore (SG) software development kit (SDK).
-
-`sbux` is named after the ticker symbol of Starbucks Corporation (SBUX) on the NASDAQ.
+`sbux` is an unofficial Starbucks Singapore (SG) Python SDK.
 
 ## Installing
 
 Install and update using `pip`;
 
 ```sh
 pip install sbux
 ```
 
-## A Simple Example
+## Example
 
 ```python
 from sbux import Starbucks
 
 
 starbucks = Starbucks
 starbucks.get_stores()
```


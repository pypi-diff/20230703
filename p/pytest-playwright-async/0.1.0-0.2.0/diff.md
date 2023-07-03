# Comparing `tmp/pytest-playwright-async-0.1.0.tar.gz` & `tmp/pytest-playwright-async-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-playwright-async-0.1.0.tar", last modified: Mon Jun 26 13:46:14 2023, max compression
+gzip compressed data, was "pytest-playwright-async-0.2.0.tar", last modified: Mon Jul  3 12:21:20 2023, max compression
```

## Comparing `pytest-playwright-async-0.1.0.tar` & `pytest-playwright-async-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:46:14.341442 pytest-playwright-async-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-26 13:46:14.341442 pytest-playwright-async-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1288 2023-06-26 13:46:03.000000 pytest-playwright-async-0.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1491 2023-06-26 13:46:04.000000 pytest-playwright-async-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 13:46:14.341442 pytest-playwright-async-0.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:46:14.341442 pytest-playwright-async-0.1.0/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 13:46:03.000000 pytest-playwright-async-0.1.0/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:46:14.341442 pytest-playwright-async-0.1.0/src/pytest_playwright_async.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-26 13:46:14.000000 pytest-playwright-async-0.1.0/src/pytest_playwright_async.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      404 2023-06-26 13:46:14.000000 pytest-playwright-async-0.1.0/src/pytest_playwright_async.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 13:46:14.000000 pytest-playwright-async-0.1.0/src/pytest_playwright_async.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-26 13:46:14.000000 pytest-playwright-async-0.1.0/src/pytest_playwright_async.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-26 13:46:14.000000 pytest-playwright-async-0.1.0/src/pytest_playwright_async.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-26 13:46:14.000000 pytest-playwright-async-0.1.0/src/pytest_playwright_async.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5958 2023-06-26 13:46:03.000000 pytest-playwright-async-0.1.0/src/pytest_playwright_async.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:46:14.341442 pytest-playwright-async-0.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)     4759 2023-06-26 13:46:03.000000 pytest-playwright-async-0.1.0/tests/test_playwright.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:21:20.764295 pytest-playwright-async-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-03 12:21:20.764295 pytest-playwright-async-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1288 2023-07-03 12:21:10.000000 pytest-playwright-async-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-07-03 12:21:10.000000 pytest-playwright-async-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 12:21:20.764295 pytest-playwright-async-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:21:20.760295 pytest-playwright-async-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:21:20.760295 pytest-playwright-async-0.2.0/src/pytest_playwright_async/
+-rw-r--r--   0 root         (0) root         (0)     5958 2023-07-03 12:21:10.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:21:20.764295 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-03 12:21:20.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      397 2023-07-03 12:21:20.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:21:20.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-03 12:21:20.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-03 12:21:20.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-03 12:21:20.000000 pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:21:20.764295 pytest-playwright-async-0.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     4759 2023-07-03 12:21:10.000000 pytest-playwright-async-0.2.0/tests/test_playwright.py
```

### Comparing `pytest-playwright-async-0.1.0/PKG-INFO` & `pytest-playwright-async-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-playwright-async
-Version: 0.1.0
+Version: 0.2.0
 Summary: ASYNC Pytest plugin for Playwright
 Author-email: m9810223 <m9810223@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/m9810223/playwright-async-pytest
 Project-URL: Source, https://github.com/m9810223/playwright-async-pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pytest-playwright-async-0.1.0/README.md` & `pytest-playwright-async-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-async-0.1.0/pyproject.toml` & `pytest-playwright-async-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "pytest-asyncio==0.20.3", # https://github.com/microsoft/playwright-python/blob/main/local-requirements.txt
 ]
 description = "ASYNC Pytest plugin for Playwright"
 license = {text = "MIT"}
 name = "pytest-playwright-async"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.1.0"
+version = "0.2.0"
 
 [project.urls]
 Homepage = "https://github.com/m9810223/playwright-async-pytest"
 Source = "https://github.com/m9810223/playwright-async-pytest"
 
 [tool.semantic_release]
 # https://python-semantic-release.readthedocs.io/en/latest/configuration.html
```

### Comparing `pytest-playwright-async-0.1.0/src/pytest_playwright_async.egg-info/PKG-INFO` & `pytest-playwright-async-0.2.0/src/pytest_playwright_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-playwright-async
-Version: 0.1.0
+Version: 0.2.0
 Summary: ASYNC Pytest plugin for Playwright
 Author-email: m9810223 <m9810223@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/m9810223/playwright-async-pytest
 Project-URL: Source, https://github.com/m9810223/playwright-async-pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pytest-playwright-async-0.1.0/src/pytest_playwright_async.py` & `pytest-playwright-async-0.2.0/src/pytest_playwright_async/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-async-0.1.0/tests/test_playwright.py` & `pytest-playwright-async-0.2.0/tests/test_playwright.py`

 * *Files identical despite different names*


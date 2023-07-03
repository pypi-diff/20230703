# Comparing `tmp/pypdtools-0.0.3.tar.gz` & `tmp/pypdtools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdtools-0.0.3.tar", last modified: Fri Jun 30 18:37:14 2023, max compression
+gzip compressed data, was "pypdtools-0.0.4.tar", last modified: Mon Jul  3 17:34:58 2023, max compression
```

## Comparing `pypdtools-0.0.3.tar` & `pypdtools-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 18:37:14.073138 pypdtools-0.0.3/
--rw-rw-rw-   0        0        0     1511 2023-06-28 17:19:48.000000 pypdtools-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2518 2023-06-30 18:37:14.072138 pypdtools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1850 2023-06-30 15:40:55.000000 pypdtools-0.0.3/README.md
--rw-rw-rw-   0        0        0     1822 2023-06-30 18:36:47.000000 pypdtools-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 18:37:14.073138 pypdtools-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 18:37:14.038129 pypdtools-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 18:37:14.045132 pypdtools-0.0.3/src/pypdtools/
--rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.3/src/pypdtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:37:14.064136 pypdtools-0.0.3/src/pypdtools/abc/
--rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.3/src/pypdtools/abc/__init__.py
--rw-rw-rw-   0        0        0      677 2023-06-28 21:28:40.000000 pypdtools-0.0.3/src/pypdtools/abc/dataframe.py
--rw-rw-rw-   0        0        0      709 2023-06-30 15:31:22.000000 pypdtools-0.0.3/src/pypdtools/abc/scripts.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:37:14.068137 pypdtools-0.0.3/src/pypdtools/core/
--rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.3/src/pypdtools/core/__init__.py
--rw-rw-rw-   0        0        0     6568 2023-06-30 15:31:22.000000 pypdtools-0.0.3/src/pypdtools/core/dataframe.py
--rw-rw-rw-   0        0        0     2627 2023-06-30 15:31:22.000000 pypdtools-0.0.3/src/pypdtools/core/scripts.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:37:14.070137 pypdtools-0.0.3/src/pypdtools/utils/
--rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.3/src/pypdtools/utils/__init__.py
--rw-rw-rw-   0        0        0     2207 2023-06-30 14:41:49.000000 pypdtools-0.0.3/src/pypdtools/utils/asyncs.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:37:14.061133 pypdtools-0.0.3/src/pypdtools.egg-info/
--rw-rw-rw-   0        0        0     2518 2023-06-30 18:37:14.000000 pypdtools-0.0.3/src/pypdtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-06-30 18:37:14.000000 pypdtools-0.0.3/src/pypdtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 18:37:14.000000 pypdtools-0.0.3/src/pypdtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      230 2023-06-30 18:37:14.000000 pypdtools-0.0.3/src/pypdtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-30 18:37:14.000000 pypdtools-0.0.3/src/pypdtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.567193 pypdtools-0.0.4/
+-rw-rw-rw-   0        0        0     1511 2023-06-28 17:19:48.000000 pypdtools-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2518 2023-07-03 17:34:58.567193 pypdtools-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1850 2023-06-30 15:40:55.000000 pypdtools-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1847 2023-07-03 17:34:08.000000 pypdtools-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 17:34:58.568194 pypdtools-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.534186 pypdtools-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.540189 pypdtools-0.0.4/src/pypdtools/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.4/src/pypdtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.559192 pypdtools-0.0.4/src/pypdtools/abc/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.4/src/pypdtools/abc/__init__.py
+-rw-rw-rw-   0        0        0      677 2023-06-28 21:28:40.000000 pypdtools-0.0.4/src/pypdtools/abc/dataframe.py
+-rw-rw-rw-   0        0        0      709 2023-06-30 15:31:22.000000 pypdtools-0.0.4/src/pypdtools/abc/scripts.py
+-rw-rw-rw-   0        0        0      430 2023-07-03 16:45:32.000000 pypdtools-0.0.4/src/pypdtools/abc/services.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.562192 pypdtools-0.0.4/src/pypdtools/core/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.4/src/pypdtools/core/__init__.py
+-rw-rw-rw-   0        0        0     6568 2023-06-30 15:31:22.000000 pypdtools-0.0.4/src/pypdtools/core/dataframe.py
+-rw-rw-rw-   0        0        0     2627 2023-06-30 15:31:22.000000 pypdtools-0.0.4/src/pypdtools/core/scripts.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.564193 pypdtools-0.0.4/src/pypdtools/core/services/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.4/src/pypdtools/core/services/__init__.py
+-rw-rw-rw-   0        0        0     2853 2023-07-03 16:45:32.000000 pypdtools-0.0.4/src/pypdtools/core/services/load_services.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.566193 pypdtools-0.0.4/src/pypdtools/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.4/src/pypdtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2207 2023-06-30 14:41:49.000000 pypdtools-0.0.4/src/pypdtools/utils/asyncs.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.555191 pypdtools-0.0.4/src/pypdtools.egg-info/
+-rw-rw-rw-   0        0        0     2518 2023-07-03 17:34:58.000000 pypdtools-0.0.4/src/pypdtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2023-07-03 17:34:58.000000 pypdtools-0.0.4/src/pypdtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 17:34:58.000000 pypdtools-0.0.4/src/pypdtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      249 2023-07-03 17:34:58.000000 pypdtools-0.0.4/src/pypdtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 17:34:58.000000 pypdtools-0.0.4/src/pypdtools.egg-info/top_level.txt
```

### Comparing `pypdtools-0.0.3/LICENSE` & `pypdtools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.3/PKG-INFO` & `pypdtools-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdtools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package with tools for pandas
 Author-email: Marciel Barcellos <marciel.barcellos@tcmrio.tc.br>
 Project-URL: source, https://github.com/msbar/pypdtools
 Project-URL: Documentation, https://msbar.github.io/pypdtools/
 Project-URL: Bug Tracker, https://github.com/msbar/pypdtools/issues
 Keywords: pandas,tools,asyncio
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypdtools Version: 0.0.3 Summary: Package with
+Metadata-Version: 2.1 Name: pypdtools Version: 0.0.4 Summary: Package with
 tools for pandas Author-email: Marciel Barcellos
 barcellos@tcmrio.tc.br> Project-URL: source, https://github.com/msbar/pypdtools
 Project-URL: Documentation, https://msbar.github.io/pypdtools/ Project-URL: Bug
 Tracker, https://github.com/msbar/pypdtools/issues Keywords:
 pandas,tools,asyncio Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `pypdtools-0.0.3/README.md` & `pypdtools-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.3/pyproject.toml` & `pypdtools-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "pypdtools"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Marciel Barcellos", email="marciel.barcellos@tcmrio.tc.br" }
 ]
 description = "Package with tools for pandas"
 
 readme = "README.md"
 requires-python = ">=3.7"
@@ -32,14 +32,15 @@
 ]
 [project.optional-dependencies]
 tests = [
   'anyio==3.6.2',
   'black==23.3.0',
   'isort==5.12.0',
   'pytest==7.3.1',
+  'sqlalchemy>=1.4.25',
 ]
 docs = [
   'mkdocs==1.4.3',
   'mkdocs-material==9.1.11',
   'mkdocstrings==0.22.0',
   'mkdocstrings-python==1.1.0',
   'pymdown-extensions==9.11',
```

### Comparing `pypdtools-0.0.3/src/pypdtools/abc/dataframe.py` & `pypdtools-0.0.4/src/pypdtools/abc/dataframe.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.3/src/pypdtools/abc/scripts.py` & `pypdtools-0.0.4/src/pypdtools/abc/scripts.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.3/src/pypdtools/core/dataframe.py` & `pypdtools-0.0.4/src/pypdtools/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.3/src/pypdtools/core/scripts.py` & `pypdtools-0.0.4/src/pypdtools/core/scripts.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.3/src/pypdtools/utils/asyncs.py` & `pypdtools-0.0.4/src/pypdtools/utils/asyncs.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.3/src/pypdtools.egg-info/PKG-INFO` & `pypdtools-0.0.4/src/pypdtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdtools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package with tools for pandas
 Author-email: Marciel Barcellos <marciel.barcellos@tcmrio.tc.br>
 Project-URL: source, https://github.com/msbar/pypdtools
 Project-URL: Documentation, https://msbar.github.io/pypdtools/
 Project-URL: Bug Tracker, https://github.com/msbar/pypdtools/issues
 Keywords: pandas,tools,asyncio
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypdtools Version: 0.0.3 Summary: Package with
+Metadata-Version: 2.1 Name: pypdtools Version: 0.0.4 Summary: Package with
 tools for pandas Author-email: Marciel Barcellos
 barcellos@tcmrio.tc.br> Project-URL: source, https://github.com/msbar/pypdtools
 Project-URL: Documentation, https://msbar.github.io/pypdtools/ Project-URL: Bug
 Tracker, https://github.com/msbar/pypdtools/issues Keywords:
 pandas,tools,asyncio Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
```


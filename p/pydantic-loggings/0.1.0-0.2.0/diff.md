# Comparing `tmp/pydantic-loggings-0.1.0.tar.gz` & `tmp/pydantic-loggings-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-loggings-0.1.0.tar", last modified: Mon Jul  3 09:38:19 2023, max compression
+gzip compressed data, was "pydantic-loggings-0.2.0.tar", last modified: Mon Jul  3 09:41:32 2023, max compression
```

## Comparing `pydantic-loggings-0.1.0.tar` & `pydantic-loggings-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:38:19.159367 pydantic-loggings-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      280 2023-07-03 09:38:19.159367 pydantic-loggings-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1205 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1744 2023-07-03 09:38:09.000000 pydantic-loggings-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 09:38:19.159367 pydantic-loggings-0.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:38:19.159367 pydantic-loggings-0.1.0/src/
--rw-r--r--   0 root         (0) root         (0)      580 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/exceptions_.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:38:19.159367 pydantic-loggings-0.1.0/src/loggings/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:38:19.159367 pydantic-loggings-0.1.0/src/loggings/base/
--rw-r--r--   0 root         (0) root         (0)      269 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/base/filters.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/base/formatters.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/base/handlers.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/base/loggers.py
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/base/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:38:19.159367 pydantic-loggings-0.1.0/src/loggings/not_set/
--rw-r--r--   0 root         (0) root         (0)      229 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/not_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/not_set/filters.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/not_set/formatters.py
--rw-r--r--   0 root         (0) root         (0)      839 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/not_set/handlers.py
--rw-r--r--   0 root         (0) root         (0)      639 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/not_set/loggers.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/loggings/not_set/logs.py
--rw-r--r--   0 root         (0) root         (0)     3724 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:38:19.159367 pydantic-loggings-0.1.0/src/pydantic_loggings.egg-info/
--rw-r--r--   0 root         (0) root         (0)      280 2023-07-03 09:38:19.000000 pydantic-loggings-0.1.0/src/pydantic_loggings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      738 2023-07-03 09:38:19.000000 pydantic-loggings-0.1.0/src/pydantic_loggings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 09:38:19.000000 pydantic-loggings-0.1.0/src/pydantic_loggings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-03 09:38:19.000000 pydantic-loggings-0.1.0/src/pydantic_loggings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-03 09:38:19.000000 pydantic-loggings-0.1.0/src/pydantic_loggings.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/types_.py
--rw-r--r--   0 root         (0) root         (0)      145 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/src/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:38:19.159367 pydantic-loggings-0.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)       72 2023-07-03 09:38:08.000000 pydantic-loggings-0.1.0/tests/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:41:32.798766 pydantic-loggings-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-07-03 09:41:32.798766 pydantic-loggings-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-07-03 09:41:20.000000 pydantic-loggings-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 09:41:32.798766 pydantic-loggings-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:41:32.794766 pydantic-loggings-0.2.0/src/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/exceptions_.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:41:32.794766 pydantic-loggings-0.2.0/src/loggings/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:41:32.794766 pydantic-loggings-0.2.0/src/loggings/base/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/base/filters.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/base/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/base/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/base/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/base/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:41:32.794766 pydantic-loggings-0.2.0/src/loggings/not_set/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/not_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/not_set/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/not_set/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/not_set/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      639 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/not_set/loggers.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/loggings/not_set/logs.py
+-rw-r--r--   0 root         (0) root         (0)     3724 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:41:32.794766 pydantic-loggings-0.2.0/src/pydantic_loggings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-07-03 09:41:32.000000 pydantic-loggings-0.2.0/src/pydantic_loggings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      738 2023-07-03 09:41:32.000000 pydantic-loggings-0.2.0/src/pydantic_loggings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 09:41:32.000000 pydantic-loggings-0.2.0/src/pydantic_loggings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-03 09:41:32.000000 pydantic-loggings-0.2.0/src/pydantic_loggings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-03 09:41:32.000000 pydantic-loggings-0.2.0/src/pydantic_loggings.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/types_.py
+-rw-r--r--   0 root         (0) root         (0)      145 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/src/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:41:32.798766 pydantic-loggings-0.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-03 09:41:19.000000 pydantic-loggings-0.2.0/tests/test_main.py
```

### Comparing `pydantic-loggings-0.1.0/README.md` & `pydantic-loggings-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.1.0/pyproject.toml` & `pydantic-loggings-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
 authors = [
   {name = "m9810223", email = "m9810223@gmail.com"},
 ]
 name = "pydantic-loggings"
+readme = "README.md"
 requires-python = ">=3.9"
-version = "0.1.0"
+version = "0.2.0"
 
 dependencies = [
   "pydantic>=2.0",
   "pydantic-settings>=2.0",
 ]
 
 [project.urls]
```

### Comparing `pydantic-loggings-0.1.0/src/__init__.py` & `pydantic-loggings-0.2.0/src/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.1.0/src/loggings/base/logs.py` & `pydantic-loggings-0.2.0/src/loggings/base/logs.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.1.0/src/loggings/not_set/formatters.py` & `pydantic-loggings-0.2.0/src/loggings/not_set/formatters.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.1.0/src/loggings/not_set/handlers.py` & `pydantic-loggings-0.2.0/src/loggings/not_set/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.1.0/src/loggings/not_set/loggers.py` & `pydantic-loggings-0.2.0/src/loggings/not_set/loggers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.1.0/src/loggings/not_set/logs.py` & `pydantic-loggings-0.2.0/src/loggings/not_set/logs.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.1.0/src/mixins.py` & `pydantic-loggings-0.2.0/src/mixins.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.1.0/src/pydantic_loggings.egg-info/SOURCES.txt` & `pydantic-loggings-0.2.0/src/pydantic_loggings.egg-info/SOURCES.txt`

 * *Files identical despite different names*


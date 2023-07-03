# Comparing `tmp/python_envparse-0.0.2.tar.gz` & `tmp/python_envparse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_envparse-0.0.2.tar", max compression
+gzip compressed data, was "python_envparse-0.0.3.tar", max compression
```

## Comparing `python_envparse-0.0.2.tar` & `python_envparse-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1069 2023-05-28 19:10:51.855849 python_envparse-0.0.2/LICENSE.txt
--rwxr-xr-x   0        0        0      339 2023-05-28 20:32:01.570121 python_envparse-0.0.2/pyproject.toml
--rwxr-xr-x   0        0        0       39 2023-05-28 18:21:33.757355 python_envparse-0.0.2/src/envparse/__init__.py
--rwxr-xr-x   0        0        0      357 2023-05-28 18:52:38.997571 python_envparse-0.0.2/src/envparse/_namespace.py
--rwxr-xr-x   0        0        0     1312 2023-05-28 20:30:56.790042 python_envparse-0.0.2/src/envparse/_parser.py
--rwxr-xr-x   0        0        0      181 2023-05-28 18:43:48.193934 python_envparse-0.0.2/src/envparse/_types.py
--rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 python_envparse-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 12:23:15.254080 python_envparse-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      339 2023-07-03 16:05:35.227622 python_envparse-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-07-01 12:23:15.254080 python_envparse-0.0.3/src/envparse/__init__.py
+-rw-r--r--   0        0        0      455 2023-07-03 16:02:59.359987 python_envparse-0.0.3/src/envparse/_namespace.py
+-rw-r--r--   0        0        0     1312 2023-07-01 12:23:15.254080 python_envparse-0.0.3/src/envparse/_parser.py
+-rw-r--r--   0        0        0      181 2023-07-01 12:23:15.254080 python_envparse-0.0.3/src/envparse/_types.py
+-rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 python_envparse-0.0.3/PKG-INFO
```

### Comparing `python_envparse-0.0.2/LICENSE.txt` & `python_envparse-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_envparse-0.0.2/src/envparse/_parser.py` & `python_envparse-0.0.3/src/envparse/_parser.py`

 * *Files identical despite different names*

### Comparing `python_envparse-0.0.2/PKG-INFO` & `python_envparse-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-envparse
-Version: 0.0.2
+Version: 0.0.3
 Summary: Argparse, but for environment variables.
 License: MIT
 Author: Rebzzel
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```


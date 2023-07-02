# Comparing `tmp/inductance-0.1.1.tar.gz` & `tmp/inductance-0.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inductance-0.1.1.tar", max compression
+gzip compressed data, was "inductance-0.1.1a3.tar", max compression
```

## Comparing `inductance-0.1.1.tar` & `inductance-0.1.1a3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-02 23:50:55.779729 inductance-0.1.1/LICENSE
--rw-r--r--   0        0        0     4348 2023-07-02 23:51:12.471840 inductance-0.1.1/README.md
--rw-r--r--   0        0        0     1807 2023-07-02 23:51:12.471840 inductance-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      151 2023-07-02 23:50:55.779729 inductance-0.1.1/src/inductance/__init__.py
--rw-r--r--   0        0        0    28091 2023-07-02 23:50:55.779729 inductance-0.1.1/src/inductance/elliptics.py
--rw-r--r--   0        0        0     4297 2023-07-02 23:50:55.779729 inductance-0.1.1/src/inductance/filaments.py
--rw-r--r--   0        0        0    34787 2023-07-02 23:50:55.779729 inductance-0.1.1/src/inductance/inductance.py
--rw-r--r--   0        0        0     5208 1970-01-01 00:00:00.000000 inductance-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-02 17:50:10.046386 inductance-0.1.1a3/LICENSE
+-rw-r--r--   0        0        0     2522 2023-07-02 17:50:10.046386 inductance-0.1.1a3/README.md
+-rw-r--r--   0        0        0     1810 2023-07-02 17:50:26.526601 inductance-0.1.1a3/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-07-02 17:50:26.526601 inductance-0.1.1a3/src/inductance/__init__.py
+-rw-r--r--   0        0        0    28091 2023-07-02 17:50:10.050387 inductance-0.1.1a3/src/inductance/elliptics.py
+-rw-r--r--   0        0        0     4297 2023-07-02 17:50:10.050387 inductance-0.1.1a3/src/inductance/filaments.py
+-rw-r--r--   0        0        0    34787 2023-07-02 17:50:10.050387 inductance-0.1.1a3/src/inductance/inductance.py
+-rw-r--r--   0        0        0     3384 1970-01-01 00:00:00.000000 inductance-0.1.1a3/PKG-INFO
```

### Comparing `inductance-0.1.1/LICENSE` & `inductance-0.1.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `inductance-0.1.1/pyproject.toml` & `inductance-0.1.1a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inductance"
-version = "0.1.1"
+version = "v0.1.1a3"
 description = "Code for 2D inductance calculations"
 authors = ["Darren Garnier <dgarnier@reinrag.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dgarnier/inductance"
 repository = "https://github.com/dgarnier/inductance"
 documentation = "https://inductance.readthedocs.io"
```

### Comparing `inductance-0.1.1/src/inductance/elliptics.py` & `inductance-0.1.1a3/src/inductance/elliptics.py`

 * *Files identical despite different names*

### Comparing `inductance-0.1.1/src/inductance/filaments.py` & `inductance-0.1.1a3/src/inductance/filaments.py`

 * *Files identical despite different names*

### Comparing `inductance-0.1.1/src/inductance/inductance.py` & `inductance-0.1.1a3/src/inductance/inductance.py`

 * *Files identical despite different names*


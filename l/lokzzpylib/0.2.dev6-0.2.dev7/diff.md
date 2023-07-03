# Comparing `tmp/lokzzpylib-0.2.dev6.tar.gz` & `tmp/lokzzpylib-0.2.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokzzpylib-0.2.dev6.tar", last modified: Mon Jul  3 09:43:49 2023, max compression
+gzip compressed data, was "lokzzpylib-0.2.dev7.tar", last modified: Mon Jul  3 09:51:47 2023, max compression
```

## Comparing `lokzzpylib-0.2.dev6.tar` & `lokzzpylib-0.2.dev7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 09:43:23.000000 lokzzpylib-0.2.dev6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 09:43:23.000000 lokzzpylib-0.2.dev6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 09:43:23.000000 lokzzpylib-0.2.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-03 09:43:23.000000 lokzzpylib-0.2.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/lokzzpylib/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-03 09:43:23.000000 lokzzpylib-0.2.dev6/lokzzpylib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/lokzzpylib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 09:43:48.000000 lokzzpylib-0.2.dev6/lokzzpylib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 09:43:48.000000 lokzzpylib-0.2.dev6/lokzzpylib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:43:48.000000 lokzzpylib-0.2.dev6/lokzzpylib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 09:43:48.000000 lokzzpylib-0.2.dev6/lokzzpylib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 09:43:48.000000 lokzzpylib-0.2.dev6/lokzzpylib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 09:43:23.000000 lokzzpylib-0.2.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:47.759672 lokzzpylib-0.2.dev7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:47.759672 lokzzpylib-0.2.dev7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:47.759672 lokzzpylib-0.2.dev7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 09:51:26.000000 lokzzpylib-0.2.dev7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 09:51:26.000000 lokzzpylib-0.2.dev7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 09:51:26.000000 lokzzpylib-0.2.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 09:51:47.759672 lokzzpylib-0.2.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-03 09:51:26.000000 lokzzpylib-0.2.dev7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:47.759672 lokzzpylib-0.2.dev7/lokzzpylib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-03 09:51:26.000000 lokzzpylib-0.2.dev7/lokzzpylib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:47.759672 lokzzpylib-0.2.dev7/lokzzpylib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 09:51:47.000000 lokzzpylib-0.2.dev7/lokzzpylib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 09:51:47.000000 lokzzpylib-0.2.dev7/lokzzpylib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:51:47.000000 lokzzpylib-0.2.dev7/lokzzpylib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 09:51:47.000000 lokzzpylib-0.2.dev7/lokzzpylib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 09:51:47.000000 lokzzpylib-0.2.dev7/lokzzpylib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 09:51:26.000000 lokzzpylib-0.2.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 09:51:47.759672 lokzzpylib-0.2.dev7/setup.cfg
```

### Comparing `lokzzpylib-0.2.dev6/.github/workflows/python-publish.yml` & `lokzzpylib-0.2.dev7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lokzzpylib-0.2.dev6/lokzzpylib/__init__.py` & `lokzzpylib-0.2.dev7/lokzzpylib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,24 +29,23 @@
 def ask_int(prompt):
     while True:
         try:
             return int(input(prompt))
         except ValueError:
             print("not a number")
 
-def printc(n, d = '', f = False, sepL = 0, sepC = ' '):
+def printc(n, d = '', f = False, sepL = 0, sepC = ' ', Beg = colored.green('//|'), BegL = 4):
     sep = ''
     for i in range(sepL):
         sep =+ sepC
-    if not f:
-        with indent(4, quote=colored.green("//|")):
-            puts(colored.blue(n) + sep + d)
-    else:
-        with indent(4, quote=colored.green("//|")):
-            puts(colored.blue(d) + sep + n)
+        with indent(BegL, quote=Beg):
+            if not f:
+                puts(colored.blue(n) + sep + d)
+            else:
+                puts(colored.blue(d) + sep + n)
 
 def clearsc():
     if name == 'nt':
         _ = system('cls')
     else:
         _ = system('clear')
```

### Comparing `lokzzpylib-0.2.dev6/pyproject.toml` & `lokzzpylib-0.2.dev7/pyproject.toml`

 * *Files identical despite different names*


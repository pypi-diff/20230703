# Comparing `tmp/lokzzpylib-0.2.dev4.tar.gz` & `tmp/lokzzpylib-0.2.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokzzpylib-0.2.dev4.tar", last modified: Sun Jul  2 04:25:02 2023, max compression
+gzip compressed data, was "lokzzpylib-0.2.dev6.tar", last modified: Mon Jul  3 09:43:49 2023, max compression
```

## Comparing `lokzzpylib-0.2.dev4.tar` & `lokzzpylib-0.2.dev6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:25:02.712719 lokzzpylib-0.2.dev4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:25:02.708719 lokzzpylib-0.2.dev4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:25:02.712719 lokzzpylib-0.2.dev4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-02 04:24:39.000000 lokzzpylib-0.2.dev4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 04:24:39.000000 lokzzpylib-0.2.dev4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 04:24:39.000000 lokzzpylib-0.2.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 04:25:02.712719 lokzzpylib-0.2.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 04:24:39.000000 lokzzpylib-0.2.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:25:02.712719 lokzzpylib-0.2.dev4/lokzzpylib/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-02 04:24:39.000000 lokzzpylib-0.2.dev4/lokzzpylib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:25:02.712719 lokzzpylib-0.2.dev4/lokzzpylib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 04:25:02.000000 lokzzpylib-0.2.dev4/lokzzpylib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-02 04:25:02.000000 lokzzpylib-0.2.dev4/lokzzpylib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:25:02.000000 lokzzpylib-0.2.dev4/lokzzpylib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 04:25:02.000000 lokzzpylib-0.2.dev4/lokzzpylib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 04:25:02.000000 lokzzpylib-0.2.dev4/lokzzpylib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-02 04:24:39.000000 lokzzpylib-0.2.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:25:02.712719 lokzzpylib-0.2.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 09:43:23.000000 lokzzpylib-0.2.dev6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 09:43:23.000000 lokzzpylib-0.2.dev6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 09:43:23.000000 lokzzpylib-0.2.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-03 09:43:23.000000 lokzzpylib-0.2.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/lokzzpylib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-03 09:43:23.000000 lokzzpylib-0.2.dev6/lokzzpylib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/lokzzpylib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 09:43:48.000000 lokzzpylib-0.2.dev6/lokzzpylib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 09:43:48.000000 lokzzpylib-0.2.dev6/lokzzpylib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:43:48.000000 lokzzpylib-0.2.dev6/lokzzpylib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 09:43:48.000000 lokzzpylib-0.2.dev6/lokzzpylib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 09:43:48.000000 lokzzpylib-0.2.dev6/lokzzpylib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 09:43:23.000000 lokzzpylib-0.2.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 09:43:49.003569 lokzzpylib-0.2.dev6/setup.cfg
```

### Comparing `lokzzpylib-0.2.dev4/.github/workflows/python-publish.yml` & `lokzzpylib-0.2.dev6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lokzzpylib-0.2.dev4/pyproject.toml` & `lokzzpylib-0.2.dev6/pyproject.toml`

 * *Files identical despite different names*


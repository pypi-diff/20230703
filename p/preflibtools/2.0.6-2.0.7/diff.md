# Comparing `tmp/preflibtools-2.0.6.tar.gz` & `tmp/preflibtools-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preflibtools-2.0.6.tar", last modified: Thu Sep 22 21:35:33 2022, max compression
+gzip compressed data, was "preflibtools-2.0.7.tar", last modified: Mon Jul  3 12:36:34 2023, max compression
```

## Comparing `preflibtools-2.0.6.tar` & `preflibtools-2.0.7.tar`

### file list

```diff
@@ -1,61 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.559727 preflibtools-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-22 21:35:25.000000 preflibtools-2.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-09-22 21:35:25.000000 preflibtools-2.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13012 2022-09-22 21:35:33.559727 preflibtools-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12100 2022-09-22 21:35:25.000000 preflibtools-2.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.555727 preflibtools-2.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.555727 preflibtools-2.0.6/docs/output/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.555727 preflibtools-2.0.6/docs/output/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/output/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/output/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/output/_static/plus.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.559727 preflibtools-2.0.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/about.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4968 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.559727 preflibtools-2.0.6/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.559727 preflibtools-2.0.6/docs/source/reference/instances/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/reference/instances/convert.rst
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/reference/instances/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/reference/instances/preflibinstance.rst
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/reference/instances/sampling.rst
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/reference/instances/sanity.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.559727 preflibtools-2.0.6/docs/source/reference/properties/
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/reference/properties/basic.rst
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/reference/properties/distance.rst
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/reference/properties/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/reference/properties/singlecrossing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/reference/properties/singlepeaked.rst
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-09-22 21:35:25.000000 preflibtools-2.0.6/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.559727 preflibtools-2.0.6/preflibtools/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-22 21:35:25.000000 preflibtools-2.0.6/preflibtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.559727 preflibtools-2.0.6/preflibtools/instances/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-22 21:35:25.000000 preflibtools-2.0.6/preflibtools/instances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-22 21:35:25.000000 preflibtools-2.0.6/preflibtools/instances/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)    40745 2022-09-22 21:35:25.000000 preflibtools-2.0.6/preflibtools/instances/preflibinstance.py
--rw-r--r--   0 runner    (1001) docker     (121)     7548 2022-09-22 21:35:25.000000 preflibtools-2.0.6/preflibtools/instances/sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     8875 2022-09-22 21:35:25.000000 preflibtools-2.0.6/preflibtools/instances/sanity.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.559727 preflibtools-2.0.6/preflibtools/properties/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-22 21:35:25.000000 preflibtools-2.0.6/preflibtools/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9932 2022-09-22 21:35:25.000000 preflibtools-2.0.6/preflibtools/properties/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2022-09-22 21:35:25.000000 preflibtools-2.0.6/preflibtools/properties/distances.py
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-09-22 21:35:25.000000 preflibtools-2.0.6/preflibtools/properties/singlecrossing.py
--rw-r--r--   0 runner    (1001) docker     (121)    31419 2022-09-22 21:35:25.000000 preflibtools-2.0.6/preflibtools/properties/singlepeakedness.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.559727 preflibtools-2.0.6/preflibtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13012 2022-09-22 21:35:33.000000 preflibtools-2.0.6/preflibtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-09-22 21:35:33.000000 preflibtools-2.0.6/preflibtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 21:35:33.000000 preflibtools-2.0.6/preflibtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 21:35:33.000000 preflibtools-2.0.6/preflibtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-22 21:35:33.000000 preflibtools-2.0.6/preflibtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-09-22 21:35:33.563727 preflibtools-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-09-22 21:35:25.000000 preflibtools-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:35:33.559727 preflibtools-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-09-22 21:35:25.000000 preflibtools-2.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22331 2022-09-22 21:35:25.000000 preflibtools-2.0.6/tests/instance.py
--rw-r--r--   0 runner    (1001) docker     (121)     5897 2022-09-22 21:35:25.000000 preflibtools-2.0.6/tests/property.py
--rw-r--r--   0 runner    (1001) docker     (121)     5827 2022-09-22 21:35:25.000000 preflibtools-2.0.6/tests/runningex.py
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-09-22 21:35:25.000000 preflibtools-2.0.6/tests/test_preflibtools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.039065 preflibtools-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 12:36:21.000000 preflibtools-2.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-03 12:36:21.000000 preflibtools-2.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-07-03 12:36:34.039065 preflibtools-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-07-03 12:36:21.000000 preflibtools-2.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.031065 preflibtools-2.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.031065 preflibtools-2.0.7/docs/output/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.031065 preflibtools-2.0.7/docs/output/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/output/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/output/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/output/_static/plus.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.031065 preflibtools-2.0.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.031065 preflibtools-2.0.7/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.035065 preflibtools-2.0.7/docs/source/reference/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/instances/convert.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/instances/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/instances/preflibinstance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/instances/sampling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/instances/sanity.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.035065 preflibtools-2.0.7/docs/source/reference/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/properties/basic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/properties/distance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/properties/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/properties/singlecrossing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/properties/singlepeaked.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.035065 preflibtools-2.0.7/preflibtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.035065 preflibtools-2.0.7/preflibtools/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/instances/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45810 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/instances/preflibinstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/instances/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/instances/sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.035065 preflibtools-2.0.7/preflibtools/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/properties/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/properties/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/properties/singlecrossing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/properties/singlepeakedness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.035065 preflibtools-2.0.7/preflibtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-07-03 12:36:33.000000 preflibtools-2.0.7/preflibtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-03 12:36:33.000000 preflibtools-2.0.7/preflibtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:36:33.000000 preflibtools-2.0.7/preflibtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:36:33.000000 preflibtools-2.0.7/preflibtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 12:36:33.000000 preflibtools-2.0.7/preflibtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-03 12:36:34.039065 preflibtools-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-03 12:36:21.000000 preflibtools-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.039065 preflibtools-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.039065 preflibtools-2.0.7/tests/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.039065 preflibtools-2.0.7/tests/instance/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/test_io_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/test_io_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/test_io_soi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/test_io_toc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/test_io_toi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/test_io_wmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/write_file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/test_categorical_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/test_order_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/runningex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/test_property.py
```

### Comparing `preflibtools-2.0.6/LICENSE.md` & `preflibtools-2.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.6/PKG-INFO` & `preflibtools-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preflibtools
-Version: 2.0.6
+Version: 2.0.7
 Summary: A set of tools to work with preference data from the PrefLib.org website.
 Home-page: https://github.com/PrefLib/preflibtools
 Author: Simon Rey
 Author-email: reysimon@orange.fr
 License: GNU General Public License v3
 Keywords: preflibtools
 Classifier: Development Status :: 5 - Production/Stable
@@ -91,18 +91,15 @@
 The most important functionality, is the ability to read and parse PrefLib data. We provide several ways to do so, as
 illustrated below.
 
 .. code-block:: python
 
     from preflibtools.instances import PrefLibInstance
 
-    # The instance can be populated either by reading a file, or from an URL.
     instance = PrefLibInstance()
-    instance.parse_file("00001-00000001.soi")
-    instance.parse_url("https://www.preflib.org/static/data/irish/00001-00000001.soi")
 
 :code:`PrefLibInstance` also stores most of the metadata about the data file.
 
 .. code-block:: python
 
     # Path to the original file, and the name of the file
     instance.file_path
```

### Comparing `preflibtools-2.0.6/README.rst` & `preflibtools-2.0.7/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -68,18 +68,15 @@
 The most important functionality, is the ability to read and parse PrefLib data. We provide several ways to do so, as
 illustrated below.
 
 .. code-block:: python
 
     from preflibtools.instances import PrefLibInstance
 
-    # The instance can be populated either by reading a file, or from an URL.
     instance = PrefLibInstance()
-    instance.parse_file("00001-00000001.soi")
-    instance.parse_url("https://www.preflib.org/static/data/irish/00001-00000001.soi")
 
 :code:`PrefLibInstance` also stores most of the metadata about the data file.
 
 .. code-block:: python
 
     # Path to the original file, and the name of the file
     instance.file_path
```

### Comparing `preflibtools-2.0.6/docs/Makefile` & `preflibtools-2.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.6/docs/make.bat` & `preflibtools-2.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.6/docs/source/conf.py` & `preflibtools-2.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.6/docs/source/index.rst` & `preflibtools-2.0.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.6/docs/source/usage.rst` & `preflibtools-2.0.7/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.6/preflibtools/instances/convert.py` & `preflibtools-2.0.7/preflibtools/instances/convert.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.6/preflibtools/instances/preflibinstance.py` & `preflibtools-2.0.7/preflibtools/instances/preflibinstance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """ This module describes the main class to deal with PrefLib instances..
 """
 import os.path
+from math import ceil
 
 from .sampling import *
 
 from copy import deepcopy
 from os import path
 
 import urllib.request
 import re
 
 
-class PrefLibInstance(object):
+class PrefLibInstance:
     """ This class provide a general template to implement specific classes representing PrefLib instances. It should
         mainly be used as an abstract class.
 
         :ivar file_path: The path to the file the instance is taken from.
         :ivar file_name: The name of the file the instance is taken from.
         :ivar data_type: The data type of the instance. Whenever a function only applies to certain types of data
             (strict and complete orders for instance), we do so by checking this value.
@@ -185,14 +186,22 @@
                     tmp = 1
                     while alt_name + "__" + str(tmp) in self.alternatives_name.values():
                         tmp += 1
                     self.alternatives_name[alt] = alt_name + "__" + str(tmp)
                 else:
                     self.alternatives_name[alt] = alt_name
 
+    def set_file_name(self, filepath):
+        """ Set self.filename according to a given filepath.
+
+            :param filepath: The filepath to a (preflib) file.
+            :type filepath: str
+        """
+        self.file_name = os.path.basename(filepath)
+
     def write(self, filepath):
         pass
 
     def write_metadata(self, file):
         """ A helper function that writes the metadata in the file.
 
             :param file: The file to write into as a file object.
@@ -253,34 +262,36 @@
                     self.num_unique_orders = int(line[23:].strip())
                 else:
                     self.parse_metadata(line, autocorrect=autocorrect)
             else:
                 break
 
         # The rest of the lines are about the preferences
-        order_pattern = re.compile(r'{[\d,]+?}|[\d,]+')
+        order_pattern = re.compile(r'\{[\d,]+?\}|[\d,]+')
         for line in lines[i:]:
-            # The first element indicates the multiplicity of the order
-            multiplicity, order_str = line.strip().split(":")
-            multiplicity = int(multiplicity)
-            order = []
-            for group in re.findall(order_pattern, order_str):
-                if group.startswith('{'):
-                    group = group[1:-1]
-                    order.append(tuple(int(alt.strip()) for alt in group.split(',') if len(alt) > 0))
+            line = "".join(line.split())
+            if len(line) > 0:
+                # The first element indicates the multiplicity of the order
+                multiplicity, order_str = line.strip().split(":")
+                multiplicity = int(multiplicity.strip())
+                order = []
+                for group in re.findall(order_pattern, order_str):
+                    if group.startswith('{'):
+                        group = group[1:-1]
+                        order.append(tuple(int(alt.strip()) for alt in group.split(',') if len(alt) > 0))
+                    else:
+                        for alt in group.split(','):
+                            if len(alt) > 0:
+                                order.append((int(alt.strip()),))
+                order = tuple(order)
+                if autocorrect and order in self.multiplicity:
+                    self.multiplicity[tuple(order)] += multiplicity
                 else:
-                    for alt in group.split(','):
-                        if len(alt) > 0:
-                            order.append((int(alt.strip()),))
-            order = tuple(order)
-            if autocorrect and order in self.multiplicity:
-                self.multiplicity[tuple(order)] += multiplicity
-            else:
-                self.orders.append(order)
-                self.multiplicity[tuple(order)] = multiplicity
+                    self.orders.append(order)
+                    self.multiplicity[tuple(order)] = multiplicity
 
         if autocorrect:
             self.num_alternatives = len(self.alternatives_name)
             self.num_unique_orders = len(self.orders)
             self.num_voters = sum(self.multiplicity.values())
 
     def parse_old(self, lines, autocorrect=False):
@@ -353,39 +364,43 @@
                 self.orders.append(order)
                 self.multiplicity[tuple(order)] = multiplicity
 
     def write(self, filepath):
         """ Writes the instance into a file whose destination has been given as argument. If no file extension is
         provided the data type of the instance is used.
 
+            Also sets `self.file_name` correctly (according to `filepath`), if `self.file_name` is empty.
+
             :param filepath: The destination where to write the instance.
             :type filepath: str
         """
         if len(path.splitext(filepath)[1]) == 0:
             filepath += "." + str(self.data_type)
-        file = open(filepath, "w", encoding="utf-8")
-        # Writing metadata in the file header
-        self.write_metadata(file)
-        file.write("# NUMBER ALTERNATIVES: {}\n# NUMBER VOTERS: {}\n# NUMBER UNIQUE ORDERS: {}\n".format(
-            self.num_alternatives, self.num_voters, self.num_unique_orders
-        ))
-        for alt, name in self.alternatives_name.items():
-            file.write("# ALTERNATIVE NAME {}: {}\n".format(alt, name))
-        # Writing the actual ballots with their multiplicity
-        orders = deepcopy(self.orders)
-        orders.sort(key=lambda o: (-self.multiplicity[o], -len(o)))
-        for order in orders:
-            order_str = ""
-            for indif_class in order:
-                if len(indif_class) == 1:
-                    order_str += str(indif_class[0]) + ","
-                else:
-                    order_str += "{" + ",".join((str(alt) for alt in indif_class)) + "},"
-            file.write("{}: {}\n".format(self.multiplicity[order], order_str[:-1]))
-        file.close()
+        # set self.filename if it is undefined
+        if not self.file_name:
+            self.set_file_name(filepath)
+        with open(filepath, "w", encoding="utf-8") as file:
+            # Writing metadata in the file header
+            self.write_metadata(file)
+            file.write("# NUMBER ALTERNATIVES: {}\n# NUMBER VOTERS: {}\n# NUMBER UNIQUE ORDERS: {}\n".format(
+                self.num_alternatives, self.num_voters, self.num_unique_orders
+            ))
+            for alt, name in self.alternatives_name.items():
+                file.write("# ALTERNATIVE NAME {}: {}\n".format(alt, name))
+            # Writing the actual ballots with their multiplicity
+            orders = deepcopy(self.orders)
+            orders.sort(key=lambda o: (-self.multiplicity[o], -len(o)))
+            for order in orders:
+                order_str = ""
+                for indif_class in order:
+                    if len(indif_class) == 1:
+                        order_str += str(indif_class[0]) + ", "
+                    else:
+                        order_str += "{" + ", ".join((str(alt) for alt in indif_class)) + "}, "
+                file.write("{}: {}\n".format(self.multiplicity[order], order_str.strip(", ")))
 
     def vote_map(self):
         """ Returns the instance described as a vote map, i.e., a dictionary whose keys are orders, mapping
             to the number of voters with the given order as their preferences. This format can be useful for some
             applications. It also ensures interoperability with the old preflibtools (vote maps were the main object).
 
             :return: A vote map representing the preferences in the instance.
@@ -574,14 +589,15 @@
             :type num_references: int
         """
         self.append_vote_map(generate_mallows_mix(num_voters, list(range(num_alternatives)), num_references))
 
     def __str__(self):
         return "Ordinal-Instance: {} <{},{}>".format(self.file_name, self.num_voters, self.num_alternatives)
 
+
 class ComparisonInstance(PrefLibInstance):
     """ To be implemented.
 
     """
 
     def __init__(self):
         PrefLibInstance.__init__(self)
@@ -645,15 +661,15 @@
             else:
                 break
 
         # The rest of the lines are about the preferences
         pref_pattern = re.compile(r'{[\d,]+?}|[\d,]+|{}')
         for line in lines[i:]:
             # The first element indicates the multiplicity of the order
-            multiplicity, pref_str = line.strip().split(":")
+            multiplicity, pref_str = line.strip().replace(" ", "").split(":")
             multiplicity = int(multiplicity)
             pref = []
             for group in re.findall(pref_pattern, pref_str):
                 if group == '{}':
                     pref.append(tuple())
                 elif group.startswith('{'):
                     group = group[1:-1]
@@ -667,51 +683,126 @@
                 self.multiplicity[tuple(pref)] += multiplicity
             else:
                 self.preferences.append(pref)
                 self.multiplicity[tuple(pref)] = multiplicity
 
         if autocorrect:
             self.num_alternatives = len(self.alternatives_name)
-            self.num_unique_preferences = len(self.preferences)
-            self.num_voters = sum(self.multiplicity.values())
+            self.recompute_cardinality_param()
+
+    def recompute_cardinality_param(self):
+        """ Recomputes the basic cardinality parameters based on the preferences list in the instance. Numbers that are
+            recomputed are the number of voters and the number of unique orders.
+        """
+        self.num_voters = sum(self.multiplicity.values())
+        self.num_unique_preferences = len(set(self.preferences))
 
     def write(self, filepath):
         """ Writes the instance into a file whose destination has been given as argument. If no file extension is
         provided the data type of the instance is used.
 
+            Also sets `self.file_name` correctly (according to `filepath`), if `self.file_name` is empty.
+
             :param filepath: The destination where to write the instance.
             :type filepath: str
         """
         if len(path.splitext(filepath)[1]) == 0:
             filepath += "." + str(self.data_type)
-        file = open(filepath, "w", encoding="utf-8")
-        # Writing metadata in the file header
-        self.write_metadata(file)
-        file.write("# NUMBER ALTERNATIVES: {}\n# NUMBER VOTERS: {}\n# NUMBER UNIQUE PREFERENCES: {}\n".format(
-            self.num_alternatives, self.num_voters, self.num_unique_preferences
-        ))
-        file.write("# NUMBER CATEGORIES: {}\n".format(self.num_categories))
-        for cat, name in self.categories_name.items():
-            file.write("# CATEGORY NAME {}: {}\n".format(cat, name))
-        for alt, name in self.alternatives_name.items():
-            file.write("# ALTERNATIVE NAME {}: {}\n".format(alt, name))
-        # Writing the actual ballots with their multiplicity
-        preferences = deepcopy(self.preferences)
-        preferences.sort(key=lambda o: (-self.multiplicity[o], -len(o)))
-        for pref in preferences:
-            pref_str = ""
-            for category in pref:
-                if len(category) == 0:
-                    pref_str += '{},'
-                elif len(category) == 1:
-                    pref_str += str(category[0]) + ","
-                else:
-                    pref_str += "{" + ",".join((str(alt) for alt in category)) + "},"
-            file.write("{}: {}\n".format(self.multiplicity[pref], pref_str[:-1]))
-        file.close()
+        # set self.filename if it is undefined
+        if not self.file_name:
+            self.set_file_name(filepath)
+        with open(filepath, "w", encoding="utf-8") as file:
+            # Writing metadata in the file header
+            self.write_metadata(file)
+            file.write("# NUMBER ALTERNATIVES: {}\n# NUMBER VOTERS: {}\n# NUMBER UNIQUE PREFERENCES: {}\n".format(
+                self.num_alternatives, self.num_voters, self.num_unique_preferences
+            ))
+            file.write("# NUMBER CATEGORIES: {}\n".format(self.num_categories))
+            for cat, name in self.categories_name.items():
+                file.write("# CATEGORY NAME {}: {}\n".format(cat, name))
+            for alt, name in self.alternatives_name.items():
+                file.write("# ALTERNATIVE NAME {}: {}\n".format(alt, name))
+            # Writing the actual ballots with their multiplicity
+            preferences = deepcopy(self.preferences)
+            preferences.sort(key=lambda o: (-self.multiplicity[o], -len(o)))
+            for pref in preferences:
+                pref_str = ""
+                for category in pref:
+                    if len(category) == 0:
+                        pref_str += '{}, '
+                    elif len(category) == 1:
+                        pref_str += str(category[0]) + ", "
+                    else:
+                        pref_str += "{" + ", ".join((str(alt) for alt in category)) + "}, "
+                file.write("{}: {}\n".format(self.multiplicity[pref], pref_str.strip(", ")))
+
+    @classmethod
+    def from_ordinal(cls, instance, size_truncators=None, relative_size_truncators=None):
+        """ Converts an ordinal instance into a categorical one. The parameters `size_truncators` and
+        `relative_size_truncators` determine where breaking points are.
+
+        :param instance: The ordinal instance.
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
+
+        :param size_truncators: List of truncation points. Each category will contains at least the truncation point
+            number of alternatives. In case of ties, all tied alternatives are in the same category. There is no need to
+             specify the last category, all additional alternatives are placed in the last one. This parameter is
+             ignored if `relative_size_truncators` is used.
+        :type size_truncators: list of int
+
+        :param relative_size_truncators: List of truncation points expressed in relative terms with respect to the total
+            number of alternatives ranked. The truncation points will thus differ for each order. All categories
+            need to be described. In case the values do not add up to one, they are normalised.
+        :type relative_size_truncators: list of float
+        """
+        if relative_size_truncators is not None and sum(relative_size_truncators) != 1:
+            total = sum(relative_size_truncators)
+            relative_size_truncators = [trunc / total for trunc in relative_size_truncators]
+        if size_truncators is None:
+            if relative_size_truncators is None:
+                raise ValueError("Both 'size_truncators' and 'relative_size_truncators' cannot be None at the same "
+                                 "time.")
+            else:
+                size_truncators = []
+        else:
+            if relative_size_truncators is None:
+                relative_size_truncators = []
+            else:
+                size_truncators = []
+
+        cat_instance = cls()
+        cat_instance.file_path = instance.file_path
+        if len(size_truncators) > 0:
+            cat_instance.num_categories = len(size_truncators) + 1
+        else:
+            cat_instance.num_categories = len(relative_size_truncators)
+        cat_instance.categories_name = {}
+        cat_instance.preferences = []
+        for order, multiplicty in instance.multiplicity.items():
+            preferences = []
+            order_index = 0
+            if len(relative_size_truncators) > 0:
+                size_truncators = [int(ceil(len(order) * truncation_point)) for truncation_point in
+                                   relative_size_truncators]
+            for truncation_point in size_truncators:
+                alts = []
+                while len(alts) < truncation_point and order_index < len(order):
+                    alts.extend(order[order_index])
+                    order_index += 1
+                preferences.append(tuple(alts))
+                if order_index >= len(order):
+                    break
+            if order_index < len(order):
+                preferences.append(tuple(a for indif_class in order[order_index:] for a in indif_class))
+            preferences = tuple(preferences)
+            cat_instance.preferences.append(preferences)
+            cat_instance.multiplicity[preferences] = multiplicty
+
+        cat_instance.num_unique_preferences = len(cat_instance.preferences)
+        return cat_instance
 
     def __str__(self):
         return "Categorical-Instance: {} <{},{}>".format(self.file_name, self.num_voters, self.num_alternatives)
 
 
 class WeightedDiGraph(object):
     """ This class is used to represent weighted directed graphs.
@@ -788,15 +879,15 @@
 
 class MatchingInstance(PrefLibInstance, WeightedDiGraph):
     """ This is the class representing a PrefLib instance for matching preferences. It basically contains the data and
         information written within a PrefLib file.
 
     """
 
-    def __init__(self, file_path = ""):
+    def __init__(self, file_path=""):
         PrefLibInstance.__init__(self)
         WeightedDiGraph.__init__(self)
         self.num_edges = 0
         self.file_path = file_path
 
         # If a filePath is given as argument, we parse it immediately
         if len(file_path) > 0:
@@ -824,15 +915,15 @@
                 else:
                     self.parse_metadata(line, autocorrect=autocorrect)
             else:
                 break
         self.num_voters = self.num_alternatives
 
         for line in lines[i:]:
-            (vertex1, vertex2, weight) = line.strip().split(",")
+            (vertex1, vertex2, weight) = line.strip().replace(" ", "").split(",")
             self.add_edge(int(vertex1), int(vertex2), float(weight))
         self.num_edges = sum(len(edge_set) for edge_set in self.node_mapping.values())
 
     def parse_old(self, lines, autocorrect=False):
         """ Parses the strings, assuming that the latter describes a graph.
 
             :param lines: A list of string, each string being one line of the instance to parse.
@@ -864,39 +955,42 @@
             self.add_edge(vertex1, vertex2, weight)
         self.num_edges = sum(len(edge_set) for edge_set in self.node_mapping.values())
 
     def write(self, filepath):
         """ Writes the instance into a file whose destination has been given as argument, assuming the instance
             represents a graph. If no file extension is provided the data type of the instance is used.
 
+            Also sets `self.file_name` correctly (according to `filepath`), if `self.file_name` is empty.
+
             :param filepath: The destination where to write the instance.
             :type filepath: str
         """
-
         if len(path.splitext(filepath)[1]) == 0:
             filepath += "." + str(self.data_type)
-        file = open(filepath, "w", encoding="utf-8")
-        # Writing metadata in the file header
-        self.write_metadata(file)
-        file.write("# NUMBER ALTERNATIVES: {}\n# NUMBER EDGES: {}\n".format(
-            self.num_alternatives, self.num_edges,
-        ))
-        for alt, name in self.alternatives_name.items():
-            file.write("# ALTERNATIVE NAME {}: {}\n".format(alt, name))
-
-        # Writing the actual graph
-        nodes = sorted(list(self.nodes()))
-        for n in nodes:
-            out_edges = sorted(list(self.outgoing_edges(n)), key=lambda x: x[1])
-            for (vertex1, vertex2, weight) in out_edges:
-                file.write("{},{},{}\n".format(vertex1, vertex2, weight))
-        file.close()
+        # set self.filename if it is undefined
+        if not self.file_name:
+            self.set_file_name(filepath)
+        with open(filepath, "w", encoding="utf-8") as file:
+            # Writing metadata in the file header
+            self.write_metadata(file)
+            file.write("# NUMBER ALTERNATIVES: {}\n# NUMBER EDGES: {}\n".format(
+                self.num_alternatives, self.num_edges,
+            ))
+            for alt, name in self.alternatives_name.items():
+                file.write("# ALTERNATIVE NAME {}: {}\n".format(alt, name))
+
+            # Writing the actual graph
+            nodes = sorted(list(self.nodes()))
+            for n in nodes:
+                out_edges = sorted(list(self.outgoing_edges(n)), key=lambda x: x[1])
+                for (vertex1, vertex2, weight) in out_edges:
+                    file.write("{}, {}, {}\n".format(vertex1, vertex2, weight))
 
     def __str__(self):
-        return "Matching-Instance: {} <{},{}>".format(self.file_name, self.num_voters, self.num_alternatives)
+        return "Matching-Instance: {} <{}, {}>".format(self.file_name, self.num_voters, self.num_alternatives)
 
 
 def get_parsed_instance(file_path):
     """ Infers from the extension of the file given as input the correct instance to use. Parses the file and return
         the instance.
 
         :param file_path: The path to the file to be parsed.
```

### Comparing `preflibtools-2.0.6/preflibtools/instances/sampling.py` & `preflibtools-2.0.7/preflibtools/instances/sampling.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ This module describes procedures to sample preferences for different probability distributions.
 """
 
 import numpy as np
 
+
 def generate_mallows(num_voters, num_alternatives, mixture, dispersions, references):
     """ Generates a profile following a mixture of Mallow's models.
 
         :param num_voters: Number of orders to sample.
         :type num_voters: int
         :param num_alternatives: Number of alternatives for the sampled orders.
         :type num_alternatives: int
@@ -63,35 +64,75 @@
 
         vote = tuple((alt,) for alt in vote)
         vote_map[vote] = vote_map.get(vote, 0) + 1
 
     return vote_map
 
 
-def generate_mallows_mix(num_voters, alternatives, num_references):
+# Given the number m of candidates and a phi\in [0,1] function computes the expected number of swaps in a vote
+# sampled from Mallows model
+def expected_number_swaps(num_candidates, phi):
+    res = phi * num_candidates / (1 - phi)
+    for j in range(1, num_candidates + 1):
+        res = res + (j * (phi ** j)) / ((phi ** j) - 1)
+    return res
+
+
+# Given the number m of candidates and a value of norm-phi\in [0,1], this function returns a value of phi such that
+# in a vote sampled from Mallows model with this parameter the expected number of swaps is a norm-phi fraction of the
+# achievable one
+def phi_from_normphi(num_candidates, normphi):
+    if normphi == 1:
+        return 1
+    exp_abs = normphi * (num_candidates * (num_candidates - 1)) / 4
+    low = 0
+    high = 1
+    while low <= high:
+        mid = (high + low) / 2
+        cur = expected_number_swaps(num_candidates, mid)
+        if abs(cur - exp_abs) < 1e-4:
+            return mid
+        # If x is greater, ignore left half
+        if cur < exp_abs:
+            low = mid
+
+        # If x is smaller, ignore right half
+        elif cur > exp_abs:
+            high = mid
+
+    # If we reach here, then the element was not present
+    return -1
+
+
+def generate_mallows_mix(num_voters, alternatives, num_references, norm_phi=True):
     """ Generates a profile following a mixture of Mallow's models for which reference points and dispersion 
         coefficients are independently and identically distributed.
 
         :param num_voters: Number of orders to sample.
         :type num_voters: int
         :param alternatives: List of alternatives for the sampled orders.
         :type alternatives: list of int
         :param num_references: Number of element
         :type num_references: int
+        :param norm_phi: Uses the normalised phi value if true, and just a uniform distribution otherwise. Defaults to True.
+        :type norm_phi: bool
 
         :return: A vote map, i.e., a dictionary whose keys are orders, mapping to the number of voters with
             the given order as their preferences.
         :rtype: dict
     """
     mixture = []
     dispersions = []
     references = []
     for i in range(num_references):
         references.append(tuple(generate_IC(1, alternatives))[0])
-        dispersions.append(round(np.random.rand(), 5))
+        phi = round(np.random.rand(), 5)
+        if norm_phi:
+            phi = phi_from_normphi(len(alternatives), phi)
+        dispersions.append(phi)
         mixture.append(np.random.randint(1, 101))
     mixture = [float(i) / float(sum(mixture)) for i in mixture]
     return generate_mallows(num_voters, len(alternatives), mixture, dispersions, references)
 
 
 def generate_urn(num_voters, alternatives, replace):
     """ Generates a profile following the urn model.
```

### Comparing `preflibtools-2.0.6/preflibtools/instances/sanity.py` & `preflibtools-2.0.7/preflibtools/instances/sanity.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.6/preflibtools/properties/basic.py` & `preflibtools-2.0.7/preflibtools/properties/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def pairwise_scores(instance):
     """ Returns a dictionary of dictionaries mapping every alternative a to the number of times it beats
         every other alternative b (the number of voters preferring a over b).
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.PreflibInstance
+        :type instance: preflibtools.instances.preflibinstance.PreflibInstance
 
         :return: A dictionary of dictionaries storing the scores.
         :rtype: dict
     """
     if instance.data_type in ["soc", "toc", "soi", "toi"]:
         scores = {alt: {a: 0 for a in instance.alternatives_name if a != alt} for alt in instance.alternatives_name}
         for order in instance.orders:
@@ -26,15 +26,15 @@
 
 
 def copeland_scores(instance):
     """ Returns a dictionary of dictionaries mapping every alternative a to their Copeland score against every other
         alternative b (the number of voters preferring a over b minus the number of voters preferring b over a).
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.PreflibInstance
+        :type instance: preflibtools.instances.preflibinstance.PreflibInstance
 
         :return: A dictionary of dictionaries storing the scores.
         :rtype: dict
     """
     if instance.data_type in ["soc", "toc", "soi", "toi"]:
         scores = {alt: {a: 0 for a in instance.alternatives_name if a != alt} for alt in instance.alternatives_name}
         for order in instance.orders:
@@ -51,15 +51,15 @@
 
 def has_condorcet(instance):
     """ Checks whether the instance has a Condorcet winner, using different procedures depending on the data type of
         the instance. An alternative is a Condorcet winner if it strictly beats every other alternative in a pairwise
         majority contest. 
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.PreflibInstance
+        :type instance: preflibtools.instances.preflibinstance.PreflibInstance
 
         :return: A boolean indicating whether the instance has a Condorcet winner or not.
         :rtype: bool
     """
     if instance.data_type in ["soc", "toc", "soi", "toi"]:
         scores = copeland_scores(instance)
         for alt, scoreDict in scores.items():
@@ -71,15 +71,15 @@
 def borda_scores(instance):
     """ Computes the total Borda scores of all the alternatives of the instance. Within an indifference class, all
         alternatives are assigned the smallest score one alternative from the class would have gotten, had the order
         been strict. For instance, for the order ({a1}, {a2, a3}, {a4}), a1 gets score 3, a2 and a3 score 1 and a4 
         score 0.
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.PreflibInstance
+        :type instance: preflibtools.instances.preflibinstance.PreflibInstance
 
         :return: A dictionary mapping every instance to their Borda score.
         :rtype: dict
     """
     if instance.data_type not in ("toc", "soc"):
         raise TypeError("You are trying to compute the Borda scores of an instance of type " +
                         str(instance.data_type) + ", this is not possible.")
@@ -97,39 +97,39 @@
     return res
 
 
 def num_alternatives(instance):
     """ Returns the number of alternatives of the instance.
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.PreflibInstance
+        :type instance: preflibtools.instances.preflibinstance.PreflibInstance
 
         :return: The number of alternatives of the instance.
         :rtype: int
     """
     return instance.num_alternatives
 
 
 def num_voters(instance):
     """ Returns the number of voters .
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.PreflibInstance
+        :type instance: preflibtools.instances.preflibinstance.PreflibInstance
 
         :return: The number of voters of the instance.
         :rtype: int
     """
     return instance.num_voters
 
 
 def num_different_preferences(instance):
     """ Returns the number of different orders of the instance.
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.PreflibInstance
+        :type instance: preflibtools.instances.preflibinstance.PreflibInstance
 
         :return: The number of different orders of the instance.
         :rtype: int
     """
     if instance.data_type in ("toc", "soc", "toi", "soi"):
         return instance.num_unique_orders
     elif instance.data_type == "cat":
@@ -137,90 +137,90 @@
 
 
 def largest_ballot(instance):
     """ Returns the size of the largest ballot of the instance, i.e., the maximum number of alternatives 
         appearing in an order.
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: The size of the largest ballot of the instance.
         :rtype: int
     """
     return max([sum([len(indif_class) for indif_class in order]) for order in instance.orders])
 
 
 def smallest_ballot(instance):
     """ Returns the size of the smallest ballot of the instance, i.e., the smallest number of alternatives 
         appearing in an order.
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: The size of the smallest ballot of the instance.
         :rtype: int
     """
     return min([sum([len(indif_class) for indif_class in order]) for order in instance.orders])
 
 
 def max_num_indif(instance):
     """ Returns the maximum number of indifference classes over the orders of the instance.
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: The maximum number of indifference classes of the instance.
         :rtype: int
     """
     return max([len([p for p in o if len(p) > 1]) for o in instance.orders] + [0])
 
 
 def min_num_indif(instance):
     """ Returns the minimum number of indifference classes over the orders of the instance.
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: The minimum number of indifference classes of the instance.
         :rtype: int
     """
     return min([len([p for p in o if len(p) > 1]) for o in instance.orders] + [instance.num_alternatives])
 
 
 def largest_indif(instance):
     """ Returns the size of the largest indifference class of any voter of the instance.
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: The size of the largest indifference class of the instance.
         :rtype: int
     """
     return max([len(p) for o in instance.orders for p in o if len(p) > 0] + [0])
 
 
 def smallest_indif(instance):
     """ Returns the size of the smallest indifference class of any voter of the instance.
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: The size of the smallest indifference class of the instance.
         :rtype: int
     """
     return min([len(p) for o in instance.orders for p in o if len(p) > 0] + [instance.num_alternatives])
 
 
 def is_approval(instance):
     """ Checks whether the instance describes an approval profile. A profile is considered to represent approval 
         ballots in two cases: All the orders are complete and consist of only two indifference classes; The orders
         are incomplete and consists of a single indifference class.
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: A boolean indicating whether the instance describes an approval profile.
         :rtype: bool
     """
     m = max([len(order) for order in instance.orders])
     if m == 1:
         return True
@@ -230,25 +230,25 @@
         return False
 
 
 def is_strict(instance):
     """ Checks whether the instance describes a profile of strict preferences.
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: A boolean indicating whether the instance describes a profile of strict preferences.
         :rtype: bool
     """
     return largest_indif(instance) == 1
 
 
 def is_complete(instance):
     """ Checks whether the instance describes a profile of complete preferences.
 
         :param instance: The instance.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: A boolean indicating whether the instance describes a profile of complete preferences.
         :rtype: bool
     """
     return smallest_ballot(instance) == instance.num_alternatives
```

### Comparing `preflibtools-2.0.6/preflibtools/properties/distances.py` & `preflibtools-2.0.7/preflibtools/properties/distances.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 
 
 def distance_matrix(instance, distance_function):
     """ Returns a matrix of the pairwise distance between all orders of the instance.
 
         :param instance: The instance to take the orders from.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
         :param distance_function: The distance function to use. It should take two orders as input.
         :type distance_function: function
 
         :return: A Numpy array of the pairwise distances, coordinates being the index of the orders in the order
             list of the instance. 
         :rtype: numpy array 
     """
```

### Comparing `preflibtools-2.0.6/preflibtools/properties/singlecrossing.py` & `preflibtools-2.0.7/preflibtools/properties/singlecrossing.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 
 
 def is_single_crossing(instance):
     """ Tests whether the instance describe a profile of single-crossed preferences.
 
         :param instance: The instance to take the orders from.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: A boolean indicating whether the instance is single-crossed or no.
         :rtype: bool
     """
 
     def prefers(a, b, o):
         return o.index(a) < o.index(b)
```

### Comparing `preflibtools-2.0.6/preflibtools/properties/singlepeakedness.py` & `preflibtools-2.0.7/preflibtools/properties/singlepeakedness.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """ This module provides procedures to deal with the potential single-peakedness of the instance.
 """
 
 import copy
 import time
 
 from itertools import combinations
-from mip import *
+
+import numpy as np
+from mip import Model, xsum, BINARY, MINIMIZE, INTEGER, OptimizationStatus
 
 
 def is_single_peaked_axis(instance, axis):
     """ Tests whether the instance is single-peaked with respect to the axis provided as argument.
 
         :param instance: the instance to work on.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
         :param axis: a list of candidates.
         :type axis: list
 
         :return: A boolean indicating if the instance is single-peaked with respect to axis.
         :rtype: bool
     """
 
@@ -59,15 +61,15 @@
     """ Tests whether the instance describes a profile of single-peaked preferences. It only works with strict
         preferences.
 
         This function implements the algorithm of Escoffier, Lang, and Ozturk (2008). We are grateful to Thor Yung 
         Pheng who developed this function (under the supervision of Umberto Grandi).
 
         :param instance: the instance to test for single-peakedness.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: The axis with respect to which the instance would be single-peaked, the empty list if the instance
             is not single-peaked.
         :rtype: list
     """
 
     if instance.data_type != "soc":
@@ -259,15 +261,15 @@
 
 def sp_cons_ones_matrix(instance):
     """ Returns a binary matrix such that the instance is single-peaked if and only if the matrix has the 
         consecutive ones property. This is an helper function to implement the algorithm proposed by Bartholdi 
         and Trick (1986) to deal with single-peakedness.
 
         :param instance: the instance to test for single-peakedness.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: A binary matrix
         :rtype: numpy array
     """
     matrix = np.zeros((sum(len(o) for o in instance.orders), instance.num_alternatives))
     matrix_index = 0
     for order in instance.orders:
@@ -380,15 +382,15 @@
 
         :param model: The ILP model, should be an instance of the python-mip Model class.
         :param left_of_vars: A list of list of python-mip variables where leftOfVars[a1][a2] is set to 1 if and only
             if a1 is to the left of a2 in the axis.
         :param voter_vars: A list of list of python-mip variables where votersVars[v] is set to 1 if and only if
             voter v is removed from consideration.
         :param instance: the instance to test for single-peakedness.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
     """
     matrix = sp_cons_ones_matrix(instance)
     voter_index = -1
     for row_index in range(len(matrix)):
         row = matrix[row_index]
         if sum(row) == 1:
             voter_index += 1
@@ -447,27 +449,28 @@
         corresponding binary matrix and then uses an ILP solver to check whether the matrix has the consecutive 
         ones property.
 
         This code is inspired by that of Zack Fitzsimmons (zfitzsim@holycross.edu) and Martin Lackner 
         (lackner@dbai.tuwien.ac.at), available at https://github.com/zmf6921/incompletesp.
 
         :param instance: the instance to test for single-peakedness.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: A triple composed of a boolean variable indicating whether the instance is single-peaked or not, 
             the python-mip optimisation status of the ILP model, and the axis for which the instance is single-peaked
             (None if the instance is not single-peaked).
         :rtype: Tuple(bool, str, list)
     """
 
     if instance.data_type not in ("toc", "soc"):
         raise TypeError("You are trying to test for single-peakedness on an instance of type " +
                         str(instance.data_type) + ", this is not possible. Only toc and soc are allowed here.")
 
     model = Model(sense=MINIMIZE)
+    model.verbose = 0
 
     init_time = time.time()
 
     left_of_vars = np.array([[model.add_var(var_type=BINARY,
                                           name='leftof_' + str(a1) + '_' + str(a2)) for a2 in
                             range(instance.num_alternatives)] for a1 in range(instance.num_alternatives)])
     pos_vars = np.array([model.add_var(var_type=INTEGER,
@@ -483,15 +486,14 @@
 
     print("Constraints for isSinglePeakedILP generated in {} seconds.".format(time.time() - init_time))
 
     init_time = time.time()
 
     # model.write('modelSP.lp')
 
-    model.verbose = 0
     model.max_gap = 0.05
     model.threads = -1
     opt_status = model.optimize()
     # if optStatus == OptimizationStatus.OPTIMAL:
     #     print('optimal solution cost {} found'.format(model.objective_value))
     # elif optStatus == OptimizationStatus.FEASIBLE:
     #     print('sol.cost {} found, best possible: {}'.format(model.objective_value, model.objective_bound))
@@ -513,15 +515,15 @@
 
 
 def approx_SP_voter_deletion_ILP(instance, weighted=False):
     """ Uses an ILP solver to compute how close to single-peakedness an instance, where closeness is measured as the 
         smallest number of voter to remove for the instance to be single-peaked.
 
         :param instance: the instance to work on.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
         :param weighted: a boolean indicating if orders in the instance should have a weight of 1 in the ILP
             optimization (the default case), or if the weight should be the number of voters having submitted
             the order. 
 
         :return: A quadruple composed of the number of voters that have been removed for the instance to be
             single-peaked, the python-mip optimisation status of the ILP model, the axis for which the instance 
             is single-peaked, and the list of voters that have been removed.
@@ -596,15 +598,15 @@
 
 
 def approx_SP_alternative_deletion_ILP(instance):
     """ Uses an ILP solver to compute how close to single-peakedness an instance, where closeness is measured as the 
         smallest number of alternatives to remove for the instance to be single-peaked.
 
         :param instance: the instance to work on.
-        :type instance: preflibtools.instance.preflibinstance.OrdinalInstance
+        :type instance: preflibtools.instances.preflibinstance.OrdinalInstance
 
         :return: A quadruple composed of the number of alternatives that have been removed for the instance to be
             single-peaked, the python-mip optimisation status of the ILP model, the axis for which the instance 
             is single-peaked, and the list of alternatives that have been removed.
         :rtype: Tuple(bool, str, list, list)
     """
```

### Comparing `preflibtools-2.0.6/preflibtools.egg-info/PKG-INFO` & `preflibtools-2.0.7/preflibtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preflibtools
-Version: 2.0.6
+Version: 2.0.7
 Summary: A set of tools to work with preference data from the PrefLib.org website.
 Home-page: https://github.com/PrefLib/preflibtools
 Author: Simon Rey
 Author-email: reysimon@orange.fr
 License: GNU General Public License v3
 Keywords: preflibtools
 Classifier: Development Status :: 5 - Production/Stable
@@ -91,18 +91,15 @@
 The most important functionality, is the ability to read and parse PrefLib data. We provide several ways to do so, as
 illustrated below.
 
 .. code-block:: python
 
     from preflibtools.instances import PrefLibInstance
 
-    # The instance can be populated either by reading a file, or from an URL.
     instance = PrefLibInstance()
-    instance.parse_file("00001-00000001.soi")
-    instance.parse_url("https://www.preflib.org/static/data/irish/00001-00000001.soi")
 
 :code:`PrefLibInstance` also stores most of the metadata about the data file.
 
 .. code-block:: python
 
     # Path to the original file, and the name of the file
     instance.file_path
```

### Comparing `preflibtools-2.0.6/preflibtools.egg-info/SOURCES.txt` & `preflibtools-2.0.7/preflibtools.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -37,11 +37,21 @@
 preflibtools/instances/sanity.py
 preflibtools/properties/__init__.py
 preflibtools/properties/basic.py
 preflibtools/properties/distances.py
 preflibtools/properties/singlecrossing.py
 preflibtools/properties/singlepeakedness.py
 tests/__init__.py
-tests/instance.py
-tests/property.py
 tests/runningex.py
-tests/test_preflibtools.py
+tests/test_property.py
+tests/instance/__init__.py
+tests/instance/test_categorical_handling.py
+tests/instance/test_order_handling.py
+tests/instance/test_sampling.py
+tests/instance/io/__init__.py
+tests/instance/io/test_io_cat.py
+tests/instance/io/test_io_instances.py
+tests/instance/io/test_io_soi.py
+tests/instance/io/test_io_toc.py
+tests/instance/io/test_io_toi.py
+tests/instance/io/test_io_wmd.py
+tests/instance/io/write_file_test.py
```

### Comparing `preflibtools-2.0.6/setup.py` & `preflibtools-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     keywords='preflibtools',
     name='preflibtools',
     packages=find_packages(),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/PrefLib/preflibtools',
-    version='2.0.6',
+    version='2.0.7',
     zip_safe=False,
 )
```

### Comparing `preflibtools-2.0.6/tests/property.py` & `preflibtools-2.0.7/tests/test_property.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,155 +1,139 @@
 from preflibtools.instances.preflibinstance import OrdinalInstance
 from preflibtools.properties.singlepeakedness import *
 from preflibtools.properties.singlecrossing import *
 from preflibtools.properties.distances import *
 from preflibtools.properties import *
 
+from unittest import TestCase
 
-def test_basic():
-    instance = OrdinalInstance()
-    orders = [((0,), (1,), (2,)), ((2,), (0,), (1,))]
-    instance.append_order_list(orders)
-    scores = borda_scores(instance)
-    assert scores[0] == 3
-    assert scores[1] == 1
-    assert scores[2] == 2
-    assert num_alternatives(instance) == 3
-    assert num_voters(instance) == 2
-    assert num_different_preferences(instance) == 2
-    assert largest_ballot(instance) == 3
-    assert smallest_ballot(instance) == 3
-    assert max_num_indif(instance) == 0
-    assert min_num_indif(instance) == 0
-    assert largest_indif(instance) == 1
-    assert smallest_indif(instance) == 1
-    assert is_approval(instance) is False
-    assert is_strict(instance) is True
-    assert is_complete(instance) is True
-    orders += [((0,), (1, 2))]
-    instance.append_order_list(orders)
-    scores = borda_scores(instance)
-    assert scores[0] == 8
-    assert scores[1] == 2
-    assert scores[2] == 4
-    assert num_alternatives(instance) == 3
-    assert num_voters(instance) == 5
-    assert num_different_preferences(instance) == 3
-    assert largest_ballot(instance) == 3
-    assert smallest_ballot(instance) == 3
-    assert max_num_indif(instance) == 1
-    assert min_num_indif(instance) == 0
-    assert largest_indif(instance) == 2
-    assert smallest_indif(instance) == 1
-    assert is_approval(instance) is False
-    assert is_strict(instance) is False
-    assert is_complete(instance) is True
-    orders += [((4, 3), (1, 2))]
-    instance.append_order_list(orders)
-    assert num_alternatives(instance) == 5
-    assert num_voters(instance) == 9
-    assert num_different_preferences(instance) == 4
-    assert largest_ballot(instance) == 4
-    assert smallest_ballot(instance) == 3
-    assert max_num_indif(instance) == 2
-    assert min_num_indif(instance) == 0
-    assert largest_indif(instance) == 2
-    assert smallest_indif(instance) == 1
-    assert is_approval(instance) is False
-    assert is_strict(instance) is False
-    assert is_complete(instance) is False
-
-    instance = OrdinalInstance()
-    instance.append_order_list([((4, 3), (1, 2)), ((1, 3), (1, 4))])
-    assert is_approval(instance) is True
-    instance.append_order_list([((2, 3), (1,)), ((3,), (1, 2))])
-    assert is_approval(instance) is False
-
-    instance = OrdinalInstance()
-    instance.append_order_list([((2, 3),), ((3,),)])
-    assert is_approval(instance) is True
-
-    instance = OrdinalInstance()
-    orders = [((0,), (1,), (2,)), ((2,), (0,), (1,)), ((1,), (2,), (0,))]
-    instance.append_order_list(orders)
-    assert has_condorcet(instance) is False
-    instance = OrdinalInstance()
-    orders = [((0,), (1,), (2,)), ((2,), (1,), (0,)), ((1,), (0,), (2,)), ((1,), (2,), (0,))]
-    instance.append_order_list(orders)
-    assert has_condorcet(instance) is True
-    instance = OrdinalInstance()
-    orders = [((0, 1), (2,), (3, 4)), ((4,), (3,), (2, 1, 0)), ((0,), (1, 3), (4,))]
-    instance.append_order_list(orders)
-    assert has_condorcet(instance) is True
-
-
-def single_peakedness_test():
-    instance = OrdinalInstance()
-    orders = [((0,), (1,), (2,)), ((2,), (0,), (1,))]
-    instance.append_order_list(orders)
-    assert is_single_peaked_axis(instance, [0, 1, 2]) is False
-    assert is_single_peaked_axis(instance, [1, 0, 2]) is True
-    assert is_single_peaked(instance)[0] is True
-    assert is_single_peaked_ILP(instance)[0] is True
-
-    instance = OrdinalInstance()
-    orders = [((0,), (1,), (2,)), ((2,), (1,), (0,)), ((1,), (0,), (2,)), ((1,), (2,), (0,))]
-    instance.append_order_list(orders)
-    assert is_single_peaked_axis(instance, [0, 1, 2]) is True
-    assert is_single_peaked_axis(instance, [1, 0, 2]) is False
-    assert is_single_peaked(instance)[0] is True
-    assert is_single_peaked(instance)[1] in ([0, 1, 2], [2, 1, 0])
-    assert is_single_peaked_ILP(instance)[0] is True
-    assert is_single_peaked_ILP(instance)[2] in ([0, 1, 2], [2, 1, 0])
-
-    instance = OrdinalInstance()
-    orders = [((0,), (1,), (2,)), ((2,), (0,), (1,)), ((1,), (2,), (0,))]
-    instance.append_order_list(orders)
-    assert is_single_peaked(instance)[0] is False
-    assert is_single_peaked_ILP(instance)[0] is False
-    assert approx_SP_voter_deletion_ILP(instance)[0] == 1
-    assert approx_SP_alternative_deletion_ILP(instance)[0] == 1
-
-    instance = OrdinalInstance()
-    orders = [((0, 1), (2,), (3, 4)), ((4,), (3,), (2, 1, 0)), ((2, 3), (1,), (0,), (4,))]
-    instance.append_order_list(orders)
-    assert is_single_peaked_ILP(instance)[0] is True
-    assert approx_SP_voter_deletion_ILP(instance)[0] == 0
-    assert approx_SP_alternative_deletion_ILP(instance)[0] == 0
-
-    instance = OrdinalInstance()
-    instance.populate_mallows_mix(30, 7, 5)
-    is_single_peaked_ILP(instance)
-    approx_SP_voter_deletion_ILP(instance)
-    approx_SP_alternative_deletion_ILP(instance)
-
-
-def single_crossing_test():
-    instance = OrdinalInstance()
-    orders = [((0,), (1,), (2,)), ((2,), (0,), (1,))]
-    instance.append_order_list(orders)
-    is_single_crossing(instance)
-
-
-def distance_test():
-    instance = OrdinalInstance()
-    orders = [((0,), (1,), (2,)), ((2,), (0,), (1,))]
-    instance.append_order_list(orders)
-    distance_matrix(instance, kendall_tau_distance)
-    distance_matrix(instance, spearman_footrule_distance)
-    distance_matrix(instance, sertel_distance)
-
-
-def main():
-    print("Test basic...")
-    test_basic()
-    print("Test single-peakedness...")
-    single_peakedness_test()
-    print("Test single-crossing...")
-    single_crossing_test()
-    print("Test distances...")
-    distance_test()
-    print("All tests successful")
 
-
-if __name__ == "__main__":
-    main()
+class TestAnalysis(TestCase):
+    def test_basic(self):
+        instance = OrdinalInstance()
+        orders = [((0,), (1,), (2,)), ((2,), (0,), (1,))]
+        instance.append_order_list(orders)
+        scores = borda_scores(instance)
+        assert scores[0] == 3
+        assert scores[1] == 1
+        assert scores[2] == 2
+        assert num_alternatives(instance) == 3
+        assert num_voters(instance) == 2
+        assert num_different_preferences(instance) == 2
+        assert largest_ballot(instance) == 3
+        assert smallest_ballot(instance) == 3
+        assert max_num_indif(instance) == 0
+        assert min_num_indif(instance) == 0
+        assert largest_indif(instance) == 1
+        assert smallest_indif(instance) == 1
+        assert is_approval(instance) is False
+        assert is_strict(instance) is True
+        assert is_complete(instance) is True
+        orders += [((0,), (1, 2))]
+        instance.append_order_list(orders)
+        scores = borda_scores(instance)
+        assert scores[0] == 8
+        assert scores[1] == 2
+        assert scores[2] == 4
+        assert num_alternatives(instance) == 3
+        assert num_voters(instance) == 5
+        assert num_different_preferences(instance) == 3
+        assert largest_ballot(instance) == 3
+        assert smallest_ballot(instance) == 3
+        assert max_num_indif(instance) == 1
+        assert min_num_indif(instance) == 0
+        assert largest_indif(instance) == 2
+        assert smallest_indif(instance) == 1
+        assert is_approval(instance) is False
+        assert is_strict(instance) is False
+        assert is_complete(instance) is True
+        orders += [((4, 3), (1, 2))]
+        instance.append_order_list(orders)
+        assert num_alternatives(instance) == 5
+        assert num_voters(instance) == 9
+        assert num_different_preferences(instance) == 4
+        assert largest_ballot(instance) == 4
+        assert smallest_ballot(instance) == 3
+        assert max_num_indif(instance) == 2
+        assert min_num_indif(instance) == 0
+        assert largest_indif(instance) == 2
+        assert smallest_indif(instance) == 1
+        assert is_approval(instance) is False
+        assert is_strict(instance) is False
+        assert is_complete(instance) is False
+
+        instance = OrdinalInstance()
+        instance.append_order_list([((4, 3), (1, 2)), ((1, 3), (1, 4))])
+        assert is_approval(instance) is True
+        instance.append_order_list([((2, 3), (1,)), ((3,), (1, 2))])
+        assert is_approval(instance) is False
+
+        instance = OrdinalInstance()
+        instance.append_order_list([((2, 3),), ((3,),)])
+        assert is_approval(instance) is True
+
+        instance = OrdinalInstance()
+        orders = [((0,), (1,), (2,)), ((2,), (0,), (1,)), ((1,), (2,), (0,))]
+        instance.append_order_list(orders)
+        assert has_condorcet(instance) is False
+        instance = OrdinalInstance()
+        orders = [((0,), (1,), (2,)), ((2,), (1,), (0,)), ((1,), (0,), (2,)), ((1,), (2,), (0,))]
+        instance.append_order_list(orders)
+        assert has_condorcet(instance) is True
+        instance = OrdinalInstance()
+        orders = [((0, 1), (2,), (3, 4)), ((4,), (3,), (2, 1, 0)), ((0,), (1, 3), (4,))]
+        instance.append_order_list(orders)
+        assert has_condorcet(instance) is True
+
+    def test_single_peakedness(self):
+        instance = OrdinalInstance()
+        orders = [((0,), (1,), (2,)), ((2,), (0,), (1,))]
+        instance.append_order_list(orders)
+        assert is_single_peaked_axis(instance, [0, 1, 2]) is False
+        assert is_single_peaked_axis(instance, [1, 0, 2]) is True
+        assert is_single_peaked(instance)[0] is True
+        assert is_single_peaked_ILP(instance)[0] is True
+
+        instance = OrdinalInstance()
+        orders = [((0,), (1,), (2,)), ((2,), (1,), (0,)), ((1,), (0,), (2,)), ((1,), (2,), (0,))]
+        instance.append_order_list(orders)
+        assert is_single_peaked_axis(instance, [0, 1, 2]) is True
+        assert is_single_peaked_axis(instance, [1, 0, 2]) is False
+        assert is_single_peaked(instance)[0] is True
+        assert is_single_peaked(instance)[1] in ([0, 1, 2], [2, 1, 0])
+        assert is_single_peaked_ILP(instance)[0] is True
+        assert is_single_peaked_ILP(instance)[2] in ([0, 1, 2], [2, 1, 0])
+
+        instance = OrdinalInstance()
+        orders = [((0,), (1,), (2,)), ((2,), (0,), (1,)), ((1,), (2,), (0,))]
+        instance.append_order_list(orders)
+        assert is_single_peaked(instance)[0] is False
+        assert is_single_peaked_ILP(instance)[0] is False
+        assert approx_SP_voter_deletion_ILP(instance)[0] == 1
+        assert approx_SP_alternative_deletion_ILP(instance)[0] == 1
+
+        instance = OrdinalInstance()
+        orders = [((0, 1), (2,), (3, 4)), ((4,), (3,), (2, 1, 0)), ((2, 3), (1,), (0,), (4,))]
+        instance.append_order_list(orders)
+        assert is_single_peaked_ILP(instance)[0] is True
+        assert approx_SP_voter_deletion_ILP(instance)[0] == 0
+        assert approx_SP_alternative_deletion_ILP(instance)[0] == 0
+
+        instance = OrdinalInstance()
+        instance.populate_mallows_mix(30, 7, 5)
+        is_single_peaked_ILP(instance)
+        approx_SP_voter_deletion_ILP(instance)
+        approx_SP_alternative_deletion_ILP(instance)
+
+    def test_single_crossing(self):
+        instance = OrdinalInstance()
+        orders = [((0,), (1,), (2,)), ((2,), (0,), (1,))]
+        instance.append_order_list(orders)
+        is_single_crossing(instance)
+
+    def test_distance(self):
+        instance = OrdinalInstance()
+        orders = [((0,), (1,), (2,)), ((2,), (0,), (1,))]
+        instance.append_order_list(orders)
+        distance_matrix(instance, kendall_tau_distance)
+        distance_matrix(instance, spearman_footrule_distance)
+        distance_matrix(instance, sertel_distance)
```

### Comparing `preflibtools-2.0.6/tests/runningex.py` & `preflibtools-2.0.7/tests/runningex.py`

 * *Files identical despite different names*


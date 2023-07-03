# Comparing `tmp/example_pkg_skop-0.0.1.tar.gz` & `tmp/example_pkg_skop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_pkg_skop-0.0.1.tar", max compression
+gzip compressed data, was "example_pkg_skop-0.0.2.tar", max compression
```

## Comparing `example_pkg_skop-0.0.1.tar` & `example_pkg_skop-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       25 2023-07-03 06:20:56.957434 example_pkg_skop-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-03 05:52:34.388918 example_pkg_skop-0.0.1/example_pkg_sk/__init__.py
--rw-r--r--   0        0        0       87 2023-07-03 05:53:57.161589 example_pkg_skop-0.0.1/example_pkg_sk/sample.py
--rw-r--r--   0        0        0      343 2023-07-03 06:17:19.741541 example_pkg_skop-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 example_pkg_skop-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-07-03 06:20:56.957434 example_pkg_skop-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 05:52:34.388918 example_pkg_skop-0.0.2/example_pkg_sk/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-03 06:27:05.773742 example_pkg_skop-0.0.2/example_pkg_sk/sample.py
+-rw-r--r--   0        0        0      343 2023-07-03 06:27:58.038352 example_pkg_skop-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 example_pkg_skop-0.0.2/PKG-INFO
```


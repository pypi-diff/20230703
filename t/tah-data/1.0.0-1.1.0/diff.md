# Comparing `tmp/tah_data-1.0.0.tar.gz` & `tmp/tah_data-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tah_data-1.0.0.tar", max compression
+gzip compressed data, was "tah_data-1.1.0.tar", max compression
```

## Comparing `tah_data-1.0.0.tar` & `tah_data-1.1.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      288 2023-06-22 10:47:32.621835 tah_data-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      467 2023-06-22 09:24:16.364151 tah_data-1.0.0/src/tah_data.py
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 tah_data-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      306 2023-07-03 11:44:01.875625 tah_data-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      564 2023-07-03 11:34:54.232946 tah_data-1.1.0/src/tah_data.py
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 tah_data-1.1.0/PKG-INFO
```


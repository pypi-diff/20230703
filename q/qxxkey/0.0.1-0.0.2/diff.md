# Comparing `tmp/qxxkey-0.0.1.tar.gz` & `tmp/qxxkey-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qxxkey-0.0.1.tar", max compression
+gzip compressed data, was "qxxkey-0.0.2.tar", max compression
```

## Comparing `qxxkey-0.0.1.tar` & `qxxkey-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      249 2023-07-03 08:43:33.565314 qxxkey-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       31 2023-07-03 08:43:26.253616 qxxkey-0.0.1/qxxkey/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 08:39:08.911479 qxxkey-0.0.1/README.md
--rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 qxxkey-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-07-03 09:25:40.643664 qxxkey-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-07-03 09:18:09.435120 qxxkey-0.0.2/qxxkey/__init__.py
+-rw-r--r--   0        0        0     1297 2023-07-03 09:24:13.078137 qxxkey-0.0.2/qxxkey/vault.py
+-rw-r--r--   0        0        0        0 2023-07-03 08:39:08.911479 qxxkey-0.0.2/README.md
+-rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 qxxkey-0.0.2/PKG-INFO
```


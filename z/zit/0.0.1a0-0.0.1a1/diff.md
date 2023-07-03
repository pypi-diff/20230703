# Comparing `tmp/zit-0.0.1a0.tar.gz` & `tmp/zit-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zit-0.0.1a0.tar", max compression
+gzip compressed data, was "zit-0.0.1a1.tar", max compression
```

## Comparing `zit-0.0.1a0.tar` & `zit-0.0.1a1.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0      318 2022-01-09 09:26:58.754966 zit-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-01-09 08:55:56.174938 zit-0.0.1a0/zit/__init__.py
--rw-r--r--   0        0        0     1014 2022-01-09 09:14:53.624955 zit-0.0.1a0/zit/zit.py
--rw-r--r--   0        0        0      505 2022-01-09 09:27:24.196264 zit-0.0.1a0/setup.py
--rw-r--r--   0        0        0      522 2022-01-09 09:27:24.196643 zit-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0      420 2022-01-09 15:40:30.445293 zit-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-01-09 08:55:56.174938 zit-0.0.1a1/zit/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-09 09:47:29.534983 zit-0.0.1a1/zit/auth.py
+-rw-r--r--   0        0        0      112 2022-01-09 15:13:01.395269 zit-0.0.1a1/zit/lambdaOpts.py
+-rw-r--r--   0        0        0      687 2022-01-09 15:18:14.935274 zit-0.0.1a1/zit/main.py
+-rw-r--r--   0        0        0      603 2022-01-09 15:40:55.094321 zit-0.0.1a1/setup.py
+-rw-r--r--   0        0        0      472 2022-01-09 15:40:55.094479 zit-0.0.1a1/PKG-INFO
```


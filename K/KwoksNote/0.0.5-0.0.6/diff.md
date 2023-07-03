# Comparing `tmp/KwoksNote-0.0.5.tar.gz` & `tmp/KwoksNote-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KwoksNote-0.0.5.tar", last modified: Mon Jul  3 07:37:54 2023, max compression
+gzip compressed data, was "KwoksNote-0.0.6.tar", last modified: Mon Jul  3 08:04:55 2023, max compression
```

## Comparing `KwoksNote-0.0.5.tar` & `KwoksNote-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 07:37:54.169370 KwoksNote-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-07-03 07:37:54.153776 KwoksNote-0.0.5/KwoksNote/
--rw-rw-rw-   0        0        0       24 2023-07-03 07:37:32.000000 KwoksNote-0.0.5/KwoksNote/__init__.py
--rw-rw-rw-   0        0        0       22 2023-07-03 07:36:23.000000 KwoksNote-0.0.5/KwoksNote/_version.py
--rw-rw-rw-   0        0        0      122 2023-07-03 07:33:20.000000 KwoksNote-0.0.5/KwoksNote/info.py
-drwxrwxrwx   0        0        0        0 2023-07-03 07:37:54.169370 KwoksNote-0.0.5/KwoksNote.egg-info/
--rw-rw-rw-   0        0        0       56 2023-07-03 07:37:54.000000 KwoksNote-0.0.5/KwoksNote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-07-03 07:37:54.000000 KwoksNote-0.0.5/KwoksNote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 07:37:54.000000 KwoksNote-0.0.5/KwoksNote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-03 07:37:54.000000 KwoksNote-0.0.5/KwoksNote.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-03 07:37:54.000000 KwoksNote-0.0.5/KwoksNote.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-03 07:37:54.169370 KwoksNote-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-07-03 07:36:15.000000 KwoksNote-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 07:37:54.169370 KwoksNote-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 08:04:55.434926 KwoksNote-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-07-03 08:04:55.434926 KwoksNote-0.0.6/KwoksNote/
+-rw-rw-rw-   0        0        0     1069 2023-07-03 07:58:24.000000 KwoksNote-0.0.6/KwoksNote/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-07-03 08:00:40.000000 KwoksNote-0.0.6/KwoksNote/_version.py
+-rw-rw-rw-   0        0        0    15838 2023-07-03 07:54:38.000000 KwoksNote-0.0.6/KwoksNote/function.py
+-rw-rw-rw-   0        0        0      122 2023-07-03 07:43:06.000000 KwoksNote-0.0.6/KwoksNote/info.py
+-rw-rw-rw-   0        0        0     1806 2023-07-03 07:56:39.000000 KwoksNote-0.0.6/KwoksNote/model.py
+-rw-rw-rw-   0        0        0      734 2023-07-03 07:50:23.000000 KwoksNote-0.0.6/KwoksNote/spider.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:04:55.434926 KwoksNote-0.0.6/KwoksNote.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-07-03 08:04:55.000000 KwoksNote-0.0.6/KwoksNote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-07-03 08:04:55.000000 KwoksNote-0.0.6/KwoksNote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 08:04:55.000000 KwoksNote-0.0.6/KwoksNote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 08:04:55.000000 KwoksNote-0.0.6/KwoksNote.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-03 08:04:55.434926 KwoksNote-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-07-03 08:01:25.000000 KwoksNote-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 08:04:55.434926 KwoksNote-0.0.6/setup.cfg
```


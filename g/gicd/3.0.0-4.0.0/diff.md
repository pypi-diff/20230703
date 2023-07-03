# Comparing `tmp/gicd-3.0.0.tar.gz` & `tmp/gicd-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gicd-3.0.0.tar", last modified: Fri Apr 16 20:33:05 2021, max compression
+gzip compressed data, was "gicd-4.0.0.tar", max compression
```

## Comparing `gicd-3.0.0.tar` & `gicd-4.0.0.tar`

### file list

```diff
@@ -1,14 +1,6 @@
-drwxr-xr-x   0 zeke       (501) staff       (20)        0 2021-04-16 20:33:05.331743 gicd-3.0.0/
--rw-r--r--   0 zeke       (501) staff       (20)     1678 2021-04-16 20:33:05.331437 gicd-3.0.0/PKG-INFO
--rw-r--r--   0 zeke       (501) staff       (20)     1027 2021-04-16 20:17:00.000000 gicd-3.0.0/README.md
-drwxr-xr-x   0 zeke       (501) staff       (20)        0 2021-04-16 20:33:05.329485 gicd-3.0.0/gicd/
--rw-r--r--   0 zeke       (501) staff       (20)       42 2021-04-16 20:33:02.000000 gicd-3.0.0/gicd/__init__.py
--rw-r--r--   0 zeke       (501) staff       (20)     2304 2021-04-16 20:31:50.000000 gicd-3.0.0/gicd/api.py
-drwxr-xr-x   0 zeke       (501) staff       (20)        0 2021-04-16 20:33:05.330991 gicd-3.0.0/gicd.egg-info/
--rw-r--r--   0 zeke       (501) staff       (20)     1678 2021-04-16 20:33:05.000000 gicd-3.0.0/gicd.egg-info/PKG-INFO
--rw-r--r--   0 zeke       (501) staff       (20)      186 2021-04-16 20:33:05.000000 gicd-3.0.0/gicd.egg-info/SOURCES.txt
--rw-r--r--   0 zeke       (501) staff       (20)        1 2021-04-16 20:33:05.000000 gicd-3.0.0/gicd.egg-info/dependency_links.txt
--rw-r--r--   0 zeke       (501) staff       (20)        8 2021-04-16 20:33:05.000000 gicd-3.0.0/gicd.egg-info/requires.txt
--rw-r--r--   0 zeke       (501) staff       (20)        5 2021-04-16 20:33:05.000000 gicd-3.0.0/gicd.egg-info/top_level.txt
--rw-r--r--   0 zeke       (501) staff       (20)       38 2021-04-16 20:33:05.331853 gicd-3.0.0/setup.cfg
--rw-r--r--   0 zeke       (501) staff       (20)      710 2021-04-16 18:22:28.000000 gicd-3.0.0/setup.py
+-rw-r--r--   0        0        0     1068 2023-04-27 02:10:07.974288 gicd-4.0.0/LICENSE
+-rw-r--r--   0        0        0     1002 2023-07-03 21:34:13.363004 gicd-4.0.0/README.md
+-rw-r--r--   0        0        0       42 2023-07-03 21:46:01.193428 gicd-4.0.0/gicd/__init__.py
+-rw-r--r--   0        0        0     2288 2023-05-26 16:58:38.602429 gicd-4.0.0/gicd/api.py
+-rw-r--r--   0        0        0     1533 2023-07-03 21:46:01.191592 gicd-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 gicd-4.0.0/PKG-INFO
```


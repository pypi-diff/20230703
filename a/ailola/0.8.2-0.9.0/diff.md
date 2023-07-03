# Comparing `tmp/ailola-0.8.2.tar.gz` & `tmp/ailola-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailola-0.8.2.tar", last modified: Mon Jul  3 08:59:59 2023, max compression
+gzip compressed data, was "ailola-0.9.0.tar", last modified: Mon Jul  3 11:08:22 2023, max compression
```

## Comparing `ailola-0.8.2.tar` & `ailola-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 08:59:59.779691 ailola-0.8.2/
--rw-r--r--   0 elhayefrat   (501) staff       (20)      197 2023-07-03 08:59:59.779775 ailola-0.8.2/PKG-INFO
--rw-r--r--   0 elhayefrat   (501) staff       (20)       16 2023-07-03 07:44:46.000000 ailola-0.8.2/README.md
-drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 08:59:59.760949 ailola-0.8.2/ailola/
--rw-r--r--   0 elhayefrat   (501) staff       (20)        0 2023-07-03 08:51:51.000000 ailola-0.8.2/ailola/__init__.py
-drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 08:59:59.779061 ailola-0.8.2/ailola/ailola.egg-info/
--rw-r--r--   0 elhayefrat   (501) staff       (20)      197 2023-07-03 08:59:59.000000 ailola-0.8.2/ailola/ailola.egg-info/PKG-INFO
--rw-r--r--   0 elhayefrat   (501) staff       (20)      288 2023-07-03 08:59:59.000000 ailola-0.8.2/ailola/ailola.egg-info/SOURCES.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)        1 2023-07-03 08:59:59.000000 ailola-0.8.2/ailola/ailola.egg-info/dependency_links.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)       38 2023-07-03 08:59:59.000000 ailola-0.8.2/ailola/ailola.egg-info/entry_points.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)       22 2023-07-03 08:59:59.000000 ailola-0.8.2/ailola/ailola.egg-info/requires.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)       16 2023-07-03 08:59:59.000000 ailola-0.8.2/ailola/ailola.egg-info/top_level.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)      236 2023-07-03 08:43:53.000000 ailola-0.8.2/ailola/ailola.py
--rw-r--r--   0 elhayefrat   (501) staff       (20)      107 2023-07-03 08:59:59.780246 ailola-0.8.2/setup.cfg
--rw-r--r--   0 elhayefrat   (501) staff       (20)      812 2023-07-03 08:59:58.000000 ailola-0.8.2/setup.py
+drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 11:08:22.683516 ailola-0.9.0/
+-rw-r--r--   0 elhayefrat   (501) staff       (20)      197 2023-07-03 11:08:22.683608 ailola-0.9.0/PKG-INFO
+-rw-r--r--   0 elhayefrat   (501) staff       (20)     2948 2023-07-03 11:06:32.000000 ailola-0.9.0/README.md
+drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 11:08:22.674376 ailola-0.9.0/ailola/
+drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 11:08:22.683183 ailola-0.9.0/ailola/ailola.egg-info/
+-rw-r--r--   0 elhayefrat   (501) staff       (20)      197 2023-07-03 11:08:22.000000 ailola-0.9.0/ailola/ailola.egg-info/PKG-INFO
+-rw-r--r--   0 elhayefrat   (501) staff       (20)      269 2023-07-03 11:08:22.000000 ailola-0.9.0/ailola/ailola.egg-info/SOURCES.txt
+-rw-r--r--   0 elhayefrat   (501) staff       (20)        1 2023-07-03 11:08:22.000000 ailola-0.9.0/ailola/ailola.egg-info/dependency_links.txt
+-rw-r--r--   0 elhayefrat   (501) staff       (20)       38 2023-07-03 11:08:22.000000 ailola-0.9.0/ailola/ailola.egg-info/entry_points.txt
+-rw-r--r--   0 elhayefrat   (501) staff       (20)       31 2023-07-03 11:08:22.000000 ailola-0.9.0/ailola/ailola.egg-info/requires.txt
+-rw-r--r--   0 elhayefrat   (501) staff       (20)        7 2023-07-03 11:08:22.000000 ailola-0.9.0/ailola/ailola.egg-info/top_level.txt
+-rw-r--r--   0 elhayefrat   (501) staff       (20)     3417 2023-07-03 10:45:15.000000 ailola-0.9.0/ailola/ailola.py
+-rw-r--r--   0 elhayefrat   (501) staff       (20)      107 2023-07-03 11:08:22.685179 ailola-0.9.0/setup.cfg
+-rw-r--r--   0 elhayefrat   (501) staff       (20)      427 2023-07-03 10:45:50.000000 ailola-0.9.0/setup.py
```


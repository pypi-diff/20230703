# Comparing `tmp/funix-0.4.2.tar.gz` & `tmp/funix-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funix-0.4.2.tar", last modified: Fri May 26 15:53:35 2023, max compression
+gzip compressed data, was "funix-0.4.3.tar", last modified: Mon Jul  3 05:40:36 2023, max compression
```

## Comparing `funix-0.4.2.tar` & `funix-0.4.3.tar`

### file list

```diff
@@ -1,65 +1,62 @@
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.387832 funix-0.4.2/
--rw-r--r--   0 yazawazi   (501) staff       (20)     1073 2023-03-14 06:41:17.000000 funix-0.4.2/LICENSE
--rw-r--r--   0 yazawazi   (501) staff       (20)       26 2023-03-14 06:41:17.000000 funix-0.4.2/MANIFEST.in
--rw-r--r--   0 yazawazi   (501) staff       (20)     8629 2023-05-26 15:53:35.387918 funix-0.4.2/PKG-INFO
--rw-r--r--   0 yazawazi   (501) staff       (20)     6748 2023-05-08 21:04:14.000000 funix-0.4.2/README.md
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.374247 funix-0.4.2/backend/
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.375825 funix-0.4.2/backend/funix/
--rw-r--r--   0 yazawazi   (501) staff       (20)     9610 2023-05-26 09:52:34.000000 funix-0.4.2/backend/funix/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4171 2023-05-23 06:01:29.000000 funix-0.4.2/backend/funix/__main__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.376679 funix-0.4.2/backend/funix/app/
--rw-r--r--   0 yazawazi   (501) staff       (20)      178 2023-05-26 11:05:26.000000 funix-0.4.2/backend/funix/app/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.377538 funix-0.4.2/backend/funix/build/
--rw-r--r--   0 yazawazi   (501) staff       (20)      326 2023-05-26 15:52:48.000000 funix-0.4.2/backend/funix/build/asset-manifest.json
--rw-r--r--   0 yazawazi   (501) staff       (20)     3870 2023-05-26 15:52:29.000000 funix-0.4.2/backend/funix/build/favicon.ico
--rw-r--r--   0 yazawazi   (501) staff       (20)      806 2023-05-26 15:52:48.000000 funix-0.4.2/backend/funix/build/index.html
--rw-r--r--   0 yazawazi   (501) staff       (20)     5347 2023-05-26 15:52:29.000000 funix-0.4.2/backend/funix/build/logo192.png
--rw-r--r--   0 yazawazi   (501) staff       (20)     9664 2023-05-26 15:52:29.000000 funix-0.4.2/backend/funix/build/logo512.png
--rw-r--r--   0 yazawazi   (501) staff       (20)      492 2023-05-26 15:52:29.000000 funix-0.4.2/backend/funix/build/manifest.json
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.374552 funix-0.4.2/backend/funix/build/static/
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.377636 funix-0.4.2/backend/funix/build/static/css/
--rw-r--r--   0 yazawazi   (501) staff       (20)     9350 2023-05-26 15:52:48.000000 funix-0.4.2/backend/funix/build/static/css/main.521e60ca.css
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.384767 funix-0.4.2/backend/funix/build/static/js/
--rw-r--r--   0 yazawazi   (501) staff       (20)  6555361 2023-05-26 15:52:48.000000 funix-0.4.2/backend/funix/build/static/js/main.72703b71.js
--rw-r--r--   0 yazawazi   (501) staff       (20)     4231 2023-05-26 15:52:48.000000 funix-0.4.2/backend/funix/build/static/js/main.72703b71.js.LICENSE.txt
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.385765 funix-0.4.2/backend/funix/build/static/media/
--rw-r--r--   0 yazawazi   (501) staff       (20)  1190211 2023-05-26 15:52:48.000000 funix-0.4.2/backend/funix/build/static/media/pdf.worker.5036a5d54184cef29958.js
--rw-r--r--   0 yazawazi   (501) staff       (20)      795 2023-05-26 15:52:48.000000 funix-0.4.2/backend/funix/build/static/media/pdf.worker.5036a5d54184cef29958.js.LICENSE.txt
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.385890 funix-0.4.2/backend/funix/config/
--rw-r--r--   0 yazawazi   (501) staff       (20)      928 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/config/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.386255 funix-0.4.2/backend/funix/decorator/
--rw-r--r--   0 yazawazi   (501) staff       (20)    50540 2023-05-26 10:58:31.000000 funix-0.4.2/backend/funix/decorator/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3113 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/decorator/file.py
--rw-r--r--   0 yazawazi   (501) staff       (20)    10936 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/decorator/magic.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.386353 funix-0.4.2/backend/funix/frontend/
--rw-r--r--   0 yazawazi   (501) staff       (20)     3462 2023-05-23 09:37:53.000000 funix-0.4.2/backend/funix/frontend/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.386547 funix-0.4.2/backend/funix/hint/
--rw-r--r--   0 yazawazi   (501) staff       (20)    10128 2023-05-26 10:49:04.000000 funix-0.4.2/backend/funix/hint/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3823 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/hint/layout.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.386714 funix-0.4.2/backend/funix/prep/
--rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 09:39:39.000000 funix-0.4.2/backend/funix/prep/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     7547 2023-05-26 10:41:26.000000 funix-0.4.2/backend/funix/prep/global_to_session.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.386813 funix-0.4.2/backend/funix/session/
--rw-r--r--   0 yazawazi   (501) staff       (20)     2310 2023-05-26 11:04:02.000000 funix-0.4.2/backend/funix/session/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.386930 funix-0.4.2/backend/funix/test/
--rw-r--r--   0 yazawazi   (501) staff       (20)     5327 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/test/test_magic.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.387030 funix-0.4.2/backend/funix/theme/
--rw-r--r--   0 yazawazi   (501) staff       (20)    10204 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/theme/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.387510 funix-0.4.2/backend/funix/util/
--rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/util/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      456 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/util/file.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      771 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/util/module.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4268 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/util/network.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      467 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/util/uri.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.387713 funix-0.4.2/backend/funix/widget/
--rw-r--r--   0 yazawazi   (501) staff       (20)     4602 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/widget/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4689 2023-05-23 03:43:55.000000 funix-0.4.2/backend/funix/widget/builtin.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-05-26 15:53:35.376550 funix-0.4.2/backend/funix.egg-info/
--rw-r--r--   0 yazawazi   (501) staff       (20)     8629 2023-05-26 15:53:35.000000 funix-0.4.2/backend/funix.egg-info/PKG-INFO
--rw-r--r--   0 yazawazi   (501) staff       (20)     1471 2023-05-26 15:53:35.000000 funix-0.4.2/backend/funix.egg-info/SOURCES.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)        1 2023-05-26 15:53:35.000000 funix-0.4.2/backend/funix.egg-info/dependency_links.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)       50 2023-05-26 15:53:35.000000 funix-0.4.2/backend/funix.egg-info/entry_points.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)      143 2023-05-26 15:53:35.000000 funix-0.4.2/backend/funix.egg-info/requires.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)        6 2023-05-26 15:53:35.000000 funix-0.4.2/backend/funix.egg-info/top_level.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)      938 2023-05-26 15:50:21.000000 funix-0.4.2/pyproject.toml
--rw-r--r--   0 yazawazi   (501) staff       (20)      114 2023-05-26 15:53:35.388174 funix-0.4.2/setup.cfg
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.216102 funix-0.4.3/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1073 2023-03-14 06:41:17.000000 funix-0.4.3/LICENSE
+-rw-r--r--   0 yazawazi   (501) staff       (20)       26 2023-03-14 06:41:17.000000 funix-0.4.3/MANIFEST.in
+-rw-r--r--   0 yazawazi   (501) staff       (20)     8629 2023-07-03 05:40:36.216215 funix-0.4.3/PKG-INFO
+-rw-r--r--   0 yazawazi   (501) staff       (20)     6748 2023-05-08 21:04:14.000000 funix-0.4.3/README.md
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.195273 funix-0.4.3/backend/
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.197441 funix-0.4.3/backend/funix/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    12587 2023-07-03 05:14:28.000000 funix-0.4.3/backend/funix/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4171 2023-05-23 06:01:29.000000 funix-0.4.3/backend/funix/__main__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.198693 funix-0.4.3/backend/funix/app/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      178 2023-05-26 11:05:26.000000 funix-0.4.3/backend/funix/app/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.200505 funix-0.4.3/backend/funix/build/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      240 2023-05-27 08:54:58.000000 funix-0.4.3/backend/funix/build/asset-manifest.json
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3870 2023-05-27 08:54:36.000000 funix-0.4.3/backend/funix/build/favicon.ico
+-rw-r--r--   0 yazawazi   (501) staff       (20)      806 2023-05-27 08:54:58.000000 funix-0.4.3/backend/funix/build/index.html
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5347 2023-05-27 08:54:36.000000 funix-0.4.3/backend/funix/build/logo192.png
+-rw-r--r--   0 yazawazi   (501) staff       (20)     9664 2023-05-27 08:54:36.000000 funix-0.4.3/backend/funix/build/logo512.png
+-rw-r--r--   0 yazawazi   (501) staff       (20)      492 2023-05-27 08:54:36.000000 funix-0.4.3/backend/funix/build/manifest.json
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.195598 funix-0.4.3/backend/funix/build/static/
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.200743 funix-0.4.3/backend/funix/build/static/css/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     9350 2023-05-27 08:54:58.000000 funix-0.4.3/backend/funix/build/static/css/main.521e60ca.css
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.205871 funix-0.4.3/backend/funix/build/static/js/
+-rw-r--r--   0 yazawazi   (501) staff       (20)  6555220 2023-05-27 08:54:58.000000 funix-0.4.3/backend/funix/build/static/js/main.ef806516.js
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4231 2023-05-27 08:54:58.000000 funix-0.4.3/backend/funix/build/static/js/main.ef806516.js.LICENSE.txt
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.206185 funix-0.4.3/backend/funix/config/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      928 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/config/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.212606 funix-0.4.3/backend/funix/decorator/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    53592 2023-06-01 23:35:40.000000 funix-0.4.3/backend/funix/decorator/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3113 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/decorator/file.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)    10936 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/decorator/magic.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.212861 funix-0.4.3/backend/funix/frontend/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3462 2023-05-23 09:37:53.000000 funix-0.4.3/backend/funix/frontend/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.213396 funix-0.4.3/backend/funix/hint/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    10668 2023-06-01 23:31:16.000000 funix-0.4.3/backend/funix/hint/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3823 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/hint/layout.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.213759 funix-0.4.3/backend/funix/prep/
+-rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 09:39:39.000000 funix-0.4.3/backend/funix/prep/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     7547 2023-05-26 10:41:26.000000 funix-0.4.3/backend/funix/prep/global_to_session.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.214094 funix-0.4.3/backend/funix/session/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2310 2023-05-26 11:04:02.000000 funix-0.4.3/backend/funix/session/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.214427 funix-0.4.3/backend/funix/test/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5327 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/test/test_magic.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.214714 funix-0.4.3/backend/funix/theme/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    10204 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/theme/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.215675 funix-0.4.3/backend/funix/util/
+-rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/util/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      456 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/util/file.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      771 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/util/module.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4268 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/util/network.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      467 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/util/uri.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.215939 funix-0.4.3/backend/funix/widget/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4602 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/widget/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4689 2023-05-23 03:43:55.000000 funix-0.4.3/backend/funix/widget/builtin.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2023-07-03 05:40:36.198581 funix-0.4.3/backend/funix.egg-info/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     8629 2023-07-03 05:40:36.000000 funix-0.4.3/backend/funix.egg-info/PKG-INFO
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1323 2023-07-03 05:40:36.000000 funix-0.4.3/backend/funix.egg-info/SOURCES.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)        1 2023-07-03 05:40:36.000000 funix-0.4.3/backend/funix.egg-info/dependency_links.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)       50 2023-07-03 05:40:36.000000 funix-0.4.3/backend/funix.egg-info/entry_points.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)      143 2023-07-03 05:40:36.000000 funix-0.4.3/backend/funix.egg-info/requires.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)        6 2023-07-03 05:40:36.000000 funix-0.4.3/backend/funix.egg-info/top_level.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)      938 2023-07-03 05:32:42.000000 funix-0.4.3/pyproject.toml
+-rw-r--r--   0 yazawazi   (501) staff       (20)      114 2023-07-03 05:40:36.216547 funix-0.4.3/setup.cfg
```

### Comparing `funix-0.4.2/LICENSE` & `funix-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/PKG-INFO` & `funix-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funix
-Version: 0.4.2
+Version: 0.4.3
 Summary: Building web apps without manually creating widgets
 Author-email: "Textea Inc." <bao@textea.co>
 License: MIT License
         
         Copyright (c) 2022-2023 Textea Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funix Version: 0.4.2 Summary: Building web apps
+Metadata-Version: 2.1 Name: funix Version: 0.4.3 Summary: Building web apps
 without manually creating widgets Author-email: "Textea Inc."
 textea.co> License: MIT License Copyright (c) 2022-2023 Textea Inc. Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `funix-0.4.2/README.md` & `funix-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/__init__.py` & `funix-0.4.3/backend/funix/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from inspect import isfunction
 from ipaddress import ip_address
 from os import listdir
 from os.path import dirname, exists, isdir, join
 from sys import exit, path
 from typing import Generator, Optional
 from urllib.parse import quote
+from flask import Flask
 
 from git import Repo
 
 import funix.decorator as decorator
 import funix.hint as hint
 from funix.app import app
 from funix.frontend import OpenFrontend, run_open_frontend, start
@@ -107,46 +108,34 @@
                 join(base_dir, file), add_to_sys_path, need_full_path
             )
         if file.endswith(".py") and file != "__init__.py":
             if need_full_path:
                 yield join(base_dir, file)
             yield file[:-3]
 
-
-def run(
+def import_from_config(
     file_or_module_name: str,
-    host: Optional[str] = "0.0.0.0",
-    port: Optional[int] = 3000,
-    no_frontend: Optional[bool] = False,
-    no_browser: Optional[bool] = False,
     lazy: Optional[bool] = False,
     dir_mode: Optional[bool] = False,
     package_mode: Optional[bool] = False,
     from_git: Optional[str] = None,
     repo_dir: Optional[str] = None,
-    no_debug: Optional[bool] = False,
     transform: Optional[bool] = False,
     app_secret: Optional[str | bool] = False,
 ) -> None:
     """
-    Run the funix app.
-    For more information, `funix -h` will help you.
+    Import files, git repos and modules from the config argument.
 
     Parameters:
         file_or_module_name (str): The file or module name to run.
-        host (str): The host to run the app on, default is "0.0.0.0"
-        port (int): The port to run the app on, default is 3000
-        no_frontend (bool): If you want to disable the frontend, default is False
-        no_browser (bool): If you want to disable the browser opening, default is False
         lazy (bool): If you want to enable lazy mode, default is False
         dir_mode (bool): If you want to enable dir mode, default is False
         package_mode (bool): If you want to enable package mode, default is False
         from_git (str): If you want to run the app from a git repo, default is None
         repo_dir (str): If you want to run the app from a git repo, you can specify the directory, default is None
-        no_debug (bool): If you want to disable debug mode, default is False
         transform (bool): If you want to enable transform mode, default is False
         app_secret (str | bool): If you want to set an app secret, default is False
 
     Returns:
         None
 
     Raises:
@@ -239,14 +228,107 @@
                     module_or_file=file_or_module_name,
                     lazy=lazy,
                     need_path=False,
                     is_module=False,
                     need_name=False,
                 )
 
+
+def get_flask_application(
+    file_or_module_name: str,
+    no_frontend: Optional[bool] = False,
+    lazy: Optional[bool] = False,
+    dir_mode: Optional[bool] = False,
+    package_mode: Optional[bool] = False,
+    from_git: Optional[str] = None,
+    repo_dir: Optional[str] = None,
+    transform: Optional[bool] = False,
+    app_secret: Optional[str | bool] = False,
+) -> Flask:
+    """
+    Get flask application for the funix app.
+
+    Parameters:
+        file_or_module_name (str): The file or module name to run.
+        no_frontend (bool): If you want to disable the frontend, default is False
+        lazy (bool): If you want to enable lazy mode, default is False
+        dir_mode (bool): If you want to enable dir mode, default is False
+        package_mode (bool): If you want to enable package mode, default is False
+        from_git (str): If you want to run the app from a git repo, default is None
+        repo_dir (str): If you want to run the app from a git repo, you can specify the directory, default is None
+        transform (bool): If you want to enable transform mode, default is False
+        app_secret (str | bool): If you want to set an app secret, default is False
+
+    Returns:
+        flask.Flask: The flask application.
+    """
+    import_from_config(
+        file_or_module_name=file_or_module_name,
+        lazy=lazy,
+        dir_mode=dir_mode,
+        package_mode=package_mode,
+        from_git=from_git,
+        repo_dir=repo_dir,
+        transform=transform,
+        app_secret=app_secret,
+    )
+
+    if not no_frontend:
+        start()
+    return app
+
+
+def run(
+    file_or_module_name: str,
+    host: Optional[str] = "0.0.0.0",
+    port: Optional[int] = 3000,
+    no_frontend: Optional[bool] = False,
+    no_browser: Optional[bool] = False,
+    lazy: Optional[bool] = False,
+    dir_mode: Optional[bool] = False,
+    package_mode: Optional[bool] = False,
+    from_git: Optional[str] = None,
+    repo_dir: Optional[str] = None,
+    no_debug: Optional[bool] = False,
+    transform: Optional[bool] = False,
+    app_secret: Optional[str | bool] = False,
+) -> None:
+    """
+    Run the funix app.
+    For more information, `funix -h` will help you.
+
+    Parameters:
+        file_or_module_name (str): The file or module name to run.
+        host (str): The host to run the app on, default is "0.0.0.0"
+        port (int): The port to run the app on, default is 3000
+        no_frontend (bool): If you want to disable the frontend, default is False
+        no_browser (bool): If you want to disable the browser opening, default is False
+        lazy (bool): If you want to enable lazy mode, default is False
+        dir_mode (bool): If you want to enable dir mode, default is False
+        package_mode (bool): If you want to enable package mode, default is False
+        from_git (str): If you want to run the app from a git repo, default is None
+        repo_dir (str): If you want to run the app from a git repo, you can specify the directory, default is None
+        no_debug (bool): If you want to disable debug mode, default is False
+        transform (bool): If you want to enable transform mode, default is False
+        app_secret (str | bool): If you want to set an app secret, default is False
+
+    Returns:
+        None
+    """
+    import_from_config(
+        file_or_module_name=file_or_module_name,
+        lazy=lazy,
+        dir_mode=dir_mode,
+        package_mode=package_mode,
+        from_git=from_git,
+        repo_dir=repo_dir,
+        transform=transform,
+        app_secret=app_secret,
+    )
+
     parsed_ip = ip_address(host)
     parsed_port = get_unused_port_from(port, parsed_ip)
 
     funix_secrets = decorator.export_secrets()
     if funix_secrets:
         local = get_compressed_ip_address_as_str(parsed_ip)
         print("Secrets:")
@@ -255,15 +337,14 @@
             print(f"Name: {name}")
             print(f"Secret: {secret}")
             if not no_frontend:
                 print(f"Link: http://{local}:{port}/{quote(name)}?secret={secret}")
             print("-" * 15)
 
     if not no_frontend:
+        start()
         print(f"Starting Funix at http://{host}:{parsed_port}")
     else:
         print(f"Starting Funix backend only at http://{host}:{parsed_port}")
     if not no_frontend and not no_browser:
-        start()
-        if not no_browser:
-            run_open_frontend(parsed_ip, parsed_port)
+        run_open_frontend(parsed_ip, parsed_port)
     app.run(host=host, port=parsed_port, debug=not no_debug)
```

### Comparing `funix-0.4.2/backend/funix/__main__.py` & `funix-0.4.3/backend/funix/__main__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/build/favicon.ico` & `funix-0.4.3/backend/funix/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/build/index.html` & `funix-0.4.3/backend/funix/build/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="description" content="Textea Funix React Frontend"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap"/><script src="https://d3js.org/d3.v5.js"></script><script src="https://mpld3.github.io/js/mpld3.v0.5.8.js"></script><title>Funix</title><script defer="defer" src="/static/js/main.72703b71.js"></script><link href="/static/css/main.521e60ca.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="description" content="Textea Funix React Frontend"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap"/><script src="https://d3js.org/d3.v5.js"></script><script src="https://mpld3.github.io/js/mpld3.v0.5.8.js"></script><title>Funix</title><script defer="defer" src="/static/js/main.ef806516.js"></script><link href="/static/css/main.521e60ca.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `funix-0.4.2/backend/funix/build/logo192.png` & `funix-0.4.3/backend/funix/build/logo192.png`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/build/logo512.png` & `funix-0.4.3/backend/funix/build/logo512.png`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/build/static/css/main.521e60ca.css` & `funix-0.4.3/backend/funix/build/static/css/main.521e60ca.css`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/build/static/js/main.72703b71.js` & `funix-0.4.3/backend/funix/build/static/js/main.ef806516.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.72703b71.js.LICENSE.txt */
+/*! For license information please see main.ef806516.js.LICENSE.txt */
 (function() {
     var __webpack_modules__ = {
             5296: function(e, t, n) {
                 "use strict";
                 n.d(t, {
                     Z: function() {
                         return ae
@@ -51680,18 +51680,14 @@
             },
             63755: function(e) {
                 "use strict";
                 e.exports = function(e) {
                     return ("number" === typeof e || "[object Number]" === Object.prototype.toString.call(e)) && e.valueOf() === e.valueOf()
                 }
             },
-            72933: function(e, t, n) {
-                "use strict";
-                e.exports = n.p + "static/media/pdf.worker.5036a5d54184cef29958.js"
-            },
             93414: function() {},
             70172: function() {},
             2001: function() {},
             33779: function() {},
             66558: function() {},
             82258: function() {},
             73897: function(e) {
@@ -52810,15 +52806,15 @@
         var n = __webpack_module_cache__[e] = {
             id: e,
             loaded: !1,
             exports: {}
         };
         return __webpack_modules__[e].call(n.exports, n, n.exports, __webpack_require__), n.loaded = !0, n.exports
     }
-    __webpack_require__.m = __webpack_modules__, __webpack_require__.n = function(e) {
+    __webpack_require__.n = function(e) {
             var t = e && e.__esModule ? function() {
                 return e.default
             } : function() {
                 return e
             };
             return __webpack_require__.d(t, {
                 a: t
@@ -52868,15 +52864,15 @@
             "undefined" !== typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
                 value: "Module"
             }), Object.defineProperty(e, "__esModule", {
                 value: !0
             })
         }, __webpack_require__.nmd = function(e) {
             return e.paths = [], e.children || (e.children = []), e
-        }, __webpack_require__.p = "/", __webpack_require__.b = document.baseURI || self.location.href;
+        };
     var __webpack_exports__ = {};
     ! function() {
         "use strict";
         var e = {};
         __webpack_require__.r(e), __webpack_require__.d(e, {
             attentionMarkers: function() {
                 return wi
@@ -100920,15 +100916,15 @@
             renderTextLayer: fl().bool,
             rotate: dj,
             scale: fl().number,
             unregisterPage: fl().func,
             width: fl().number
         });
         var Qj = n.forwardRef(Xj);
-        NN(!WN, "Loading PDF.js worker may not work on protocols other than HTTP/HTTPS. ".concat(QN)), AN.GlobalWorkerOptions.workerSrc = new URL(__webpack_require__(72933), __webpack_require__.b), AN.GlobalWorkerOptions.workerSrc = "//cdn.jsdelivr.net/npm/pdfjs-dist@".concat(AN.version, "/build/pdf.worker.min.js");
+        NN(!WN, "Loading PDF.js worker may not work on protocols other than HTTP/HTTPS. ".concat(QN)), AN.GlobalWorkerOptions.workerSrc = "pdf.worker.js", AN.GlobalWorkerOptions.workerSrc = "//cdn.jsdelivr.net/npm/pdfjs-dist@".concat(AN.version, "/build/pdf.worker.min.js");
         var Jj = function(e) {
             var t = n.useState(0),
                 r = (0, o.Z)(t, 2),
                 a = r[0],
                 c = r[1],
                 i = n.useState(1),
                 l = (0, o.Z)(i, 2),
@@ -100963,16 +100959,27 @@
                     alignItems: "center",
                     children: (0, f.jsx)(zj, {
                         file: e.pdf,
                         onLoadSuccess: function(e) {
                             var t = e.numPages;
                             c(t)
                         },
+                        onItemClick: function(e) {
+                            var t = e.pageNumber;
+                            try {
+                                var n = parseInt(t);
+                                u(n)
+                            } catch (r) {
+                                console.error(r)
+                            }
+                        },
                         children: (0, f.jsx)(Qj, {
-                            pageNumber: s
+                            pageNumber: s,
+                            scale: 1.5,
+                            renderMode: "canvas"
                         })
                     })
                 })]
             })
         };
 
         function eB(e) {
```

### Comparing `funix-0.4.2/backend/funix/build/static/js/main.72703b71.js.LICENSE.txt` & `funix-0.4.3/backend/funix/build/static/js/main.ef806516.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/config/__init__.py` & `funix-0.4.3/backend/funix/config/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/decorator/__init__.py` & `funix-0.4.3/backend/funix/decorator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Funix decorator. The central logic of Funix.
 """
+from copy import deepcopy
 from functools import wraps
 from importlib import import_module
 from inspect import Parameter, Signature, getsource, signature
 from json import dumps
 from secrets import token_hex
 from traceback import format_exc
 from types import ModuleType
@@ -38,18 +39,20 @@
     ExamplesType,
     InputLayout,
     LabelsType,
     OutputLayout,
     SessionVariablesType,
     TreatAsType,
     WhitelistType,
-    WidgetsType,
+    WidgetsType, PreFillType, PreFillEmpty,
 )
 from funix.theme import get_dict_theme, parse_theme
 from funix.widget import generate_frontend_widget_config
+from funix.session import set_global_variable, get_global_variable
+
 
 __matplotlib_use = False
 """
 Whether Funix can handle matplotlib-related logic
 """
 
 try:
@@ -107,14 +110,22 @@
 
 __app_secret: str | None = None
 """
 App secret, for all functions.
 """
 
 mpld3: ModuleType | None = None
+"""
+The mpld3 module.
+"""
+
+pre_fill_metadata: dict[str, list[str | int | PreFillEmpty]] = {}
+"""
+A dict, key is function name, value is a list of indexes/keys of pre-fill parameters.
+"""
 
 
 def set_function_secret(secret: str, function_id: str, function_name: str) -> None:
     """
     Set the secret of a function.
 
     Parameters:
@@ -245,14 +256,15 @@
     examples: ExamplesType = None,
     argument_labels: LabelsType = None,
     input_layout: InputLayout = None,
     output_layout: OutputLayout = None,
     conditional_visible: ConditionalVisibleType = None,
     argument_config: ArgumentConfigType = None,
     session_variables: SessionVariablesType = None,
+    pre_fill: PreFillType = None,
     __full_module: Optional[str] = None,
 ):
     """
     Decorator for functions to convert them to web apps
     The heart of Funix, all the beginning of the magic happens here
     (or at least most of it lol)
 
@@ -276,25 +288,26 @@
         examples(ExamplesType): examples for parameters
         argument_labels(LabelsType): labels for parameters
         input_layout(InputLayout): layout for input widgets
         output_layout(OutputLayout): layout for output widgets
         conditional_visible(ConditionalVisibleType): conditional visibility for widgets
         argument_config(ArgumentConfigType): config for widgets
         session_variables(SessionVariablesType): session variables for functions
+        pre_fill(PreFillType): pre-fill values for parameters
         __full_module(str):
             full module path of the function, for `path` only.
             You don't need to set it unless you are funixing a directory and package.
 
     Returns:
         function: the decorated function
 
     Raises:
         Check code for details
     """
-    global __parsed_themes
+    global __parsed_themes, pre_fill_metadata
 
     def decorator(function: callable) -> callable:
         """
         Decorator for functions to convert them to web apps
 
         Parameters:
             function(callable): the function to be decorated
@@ -531,14 +544,30 @@
                         row_item_done.pop("code")
                     elif "index" in row_item:
                         row_item_done["type"] = "index"
                         return_output_indexes.append(row_item_done["index"])
                     row_layout.append(row_item_done)
                 return_output_layout.append(row_layout)
 
+            if pre_fill:
+                for _, from_arg_function_info in pre_fill.items():
+                    if isinstance(from_arg_function_info, tuple):
+                        from_arg_function_name = getattr(from_arg_function_info[0], "__name__")
+                        from_arg_function_index_or_key = from_arg_function_info[1]
+                        if from_arg_function_name in pre_fill_metadata:
+                            pre_fill_metadata[from_arg_function_name].append(from_arg_function_index_or_key)
+                        else:
+                            pre_fill_metadata[from_arg_function_name] = [from_arg_function_index_or_key]
+                    else:
+                        from_arg_function_name = getattr(from_arg_function_info, "__name__")
+                        if from_arg_function_name in pre_fill_metadata:
+                            pre_fill_metadata[from_arg_function_name].append(PreFillEmpty)
+                        else:
+                            pre_fill_metadata[from_arg_function_name] = [PreFillEmpty]
+
             def create_decorated_params(arg_name: str) -> None:
                 """
                 Creates a decorated_params entry for the given arg_name if it doesn't exist
 
                 Parameters:
                     arg_name (str): The name of the argument
                 """
@@ -830,33 +859,27 @@
                     config["required"].append(then_item)
                     delete_keys.add(then_item)
                 all_of.append(config)
 
             for key in delete_keys:
                 json_schema_props.pop(key)
 
-            keep_ordered_list = list(function_signature.parameters.keys())
-            keep_ordered_dict = {}
-            for key in keep_ordered_list:
-                if key in json_schema_props.keys():
-                    keep_ordered_dict[key] = json_schema_props[key]
-
             decorated_function = {
                 "id": function_id,
                 "name": function_name,
                 "params": decorated_params,
                 "theme": parsed_theme[4],
                 "return_type": return_type_parsed,
                 "description": function_description,
                 "direction": function_direction,
                 "schema": {
                     "title": function_title,
                     "description": function_description,
                     "type": "object",
-                    "properties": keep_ordered_dict,
+                    "properties": json_schema_props,
                     "allOf": all_of,
                     "input_layout": return_input_layout,
                     "output_layout": return_output_layout,
                     "output_indexes": return_output_indexes,
                 },
                 "destination": destination,
                 "source": source_code,
@@ -872,14 +895,29 @@
                 Routes:
                     /param/{endpoint}
                     /param/{function_id}
 
                 Returns:
                     flask.Response: The function's parameters
                 """
+                if pre_fill is not None:
+                    new_decorated_function = deepcopy(decorated_function)
+                    for argument_key, from_function_info in pre_fill.items():
+                        if isinstance(from_function_info, tuple):
+                            last_result = get_global_variable(
+                                getattr(from_function_info[0], "__name__") + f"_{from_function_info[1]}"
+                            )
+                        else:
+                            last_result = get_global_variable(
+                                getattr(from_function_info, "__name__") + "_result"
+                            )
+                        if last_result is not None:
+                            new_decorated_function["params"][argument_key]["default"] = last_result
+                            new_decorated_function["schema"]["properties"][argument_key]["default"] = last_result
+                    return Response(dumps(new_decorated_function), mimetype="application/json")
                 return Response(dumps(decorated_function), mimetype="application/json")
 
             decorated_function_param_getter.__setattr__(
                 "__name__", f"{function_name}_param_getter"
             )
             get_wrapper_endpoint(decorated_function_param_getter)
             get_wrapper_id(decorated_function_param_getter)
@@ -986,88 +1024,97 @@
                     @wraps(function)
                     def wrapped_function(**wrapped_function_kwargs):
                         """
                         The function's wrapper
                         """
                         # TODO: Best result handling, refactor it if possible
                         try:
+                            function_call_result = function(**wrapped_function_kwargs)
+                            function_call_name = getattr(function, "__name__")
+                            if function_call_name in pre_fill_metadata:
+                                for index_or_key in pre_fill_metadata[function_call_name]:
+                                    if index_or_key is PreFillEmpty:
+                                        set_global_variable(function_call_name + "_result", function_call_result)
+                                    else:
+                                        set_global_variable(
+                                            function_call_name + f"_{index_or_key}",
+                                            function_call_result[index_or_key]
+                                        )
                             if return_type_parsed == "Figure":
-                                fig = function(**wrapped_function_kwargs)
-                                return [get_figure(fig)]
+                                return [get_figure(function_call_result)]
                             if return_type_parsed in supported_basic_file_types:
                                 return [
-                                    get_static_uri(function(**wrapped_function_kwargs))
+                                    get_static_uri(function_call_result)
                                 ]
                             else:
-                                function_result = function(**wrapped_function_kwargs)
-                                if isinstance(function_result, list):
-                                    return [function_result]
-                                if not isinstance(function_result, (str, dict, tuple)):
-                                    function_result = dumps(function_result)
+                                if isinstance(function_call_result, list):
+                                    return [function_call_result]
+                                if not isinstance(function_call_result, (str, dict, tuple)):
+                                    function_call_result = dumps(function_call_result)
                                 if cast_to_list_flag:
-                                    function_result = list(function_result)
+                                    function_call_result = list(function_call_result)
                                 else:
-                                    if isinstance(function_result, (str, dict)):
-                                        function_result = [function_result]
-                                    if isinstance(function_result, tuple):
-                                        function_result = list(function_result)
-                                if function_result and isinstance(
-                                    function_result, list
+                                    if isinstance(function_call_result, (str, dict)):
+                                        function_call_result = [function_call_result]
+                                    if isinstance(function_call_result, tuple):
+                                        function_call_result = list(function_call_result)
+                                if function_call_result and isinstance(
+                                    function_call_result, list
                                 ):
                                     if isinstance(return_type_parsed, list):
                                         for position, single_return_type in enumerate(
                                             return_type_parsed
                                         ):
                                             if single_return_type == "Figure":
-                                                function_result[position] = get_figure(
-                                                    function_result[position]
+                                                function_call_result[position] = get_figure(
+                                                    function_call_result[position]
                                                 )
                                             if (
                                                 single_return_type
                                                 in supported_basic_file_types
                                             ):
                                                 if (
-                                                    type(function_result[position])
+                                                    type(function_call_result[position])
                                                     == "list"
                                                 ):
-                                                    function_result[position] = [
+                                                    function_call_result[position] = [
                                                         get_static_uri(single)
-                                                        for single in function_result[
+                                                        for single in function_call_result[
                                                             position
                                                         ]
                                                     ]
                                                 else:
-                                                    function_result[
+                                                    function_call_result[
                                                         position
                                                     ] = get_static_uri(
-                                                        function_result[position]
+                                                        function_call_result[position]
                                                     )
-                                        return function_result
+                                        return function_call_result
                                     else:
                                         if return_type_parsed == "Figure":
-                                            function_result = [
-                                                get_figure(function_result[0])
+                                            function_call_result = [
+                                                get_figure(function_call_result[0])
                                             ]
                                         if (
                                             return_type_parsed
                                             in supported_basic_file_types
                                         ):
-                                            if type(function_result[0]) == "list":
-                                                function_result = [
+                                            if type(function_call_result[0]) == "list":
+                                                function_call_result = [
                                                     [
                                                         get_static_uri(single)
-                                                        for single in function_result[0]
+                                                        for single in function_call_result[0]
                                                     ]
                                                 ]
                                             else:
-                                                function_result = [
-                                                    get_static_uri(function_result[0])
+                                                function_call_result = [
+                                                    get_static_uri(function_call_result[0])
                                                 ]
-                                        return function_result
-                                return function_result
+                                        return function_call_result
+                                return function_call_result
                         except:
                             return {
                                 "error_type": "function",
                                 "error_body": format_exc(),
                             }
 
                     cell_names = []
```

### Comparing `funix-0.4.2/backend/funix/decorator/file.py` & `funix-0.4.3/backend/funix/decorator/file.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/decorator/magic.py` & `funix-0.4.3/backend/funix/decorator/magic.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/frontend/__init__.py` & `funix-0.4.3/backend/funix/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/hint/__init__.py` & `funix-0.4.3/backend/funix/hint/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This file is used to define the type hint of the Funix backend.
 """
 
-from typing import Literal, NewType, Optional, TypeAlias, TypedDict
+from typing import Literal, NewType, Optional, TypeAlias, TypedDict, TypeVar, Callable
 
 from funix.hint.layout import InputRow, OutputRow
 from funix.widget import builtin
 
 DestinationType = Optional[Literal["column", "row", "sheet"]]
 """
 For yodas only, the destination of the page.
@@ -219,14 +219,34 @@
 """
 The type of the `session_variables`.
 
 Examples:
     ["a", "b"] -> The session variables: `a`, `b` will be saved.
 """
 
+PreFillArgumentFrom = Callable | tuple[Callable, int]
+"""
+Pre-fill argument from.
+
+Types:
+    callable: The function.
+    tuple[callable, int]: The function and the index.
+"""
+
+PreFillType = Optional[dict[str, PreFillArgumentFrom]]
+"""
+The type of the `pre_fill`.
+
+Examples:
+    {"a": "b"} -> The parameter `a` will be pre-filled from the function `b`'s result.
+    {"a": ("b", 1)} -> The parameter `a` will be pre-filled from the function `b`'s result, and the index is `1`.
+"""
+
+PreFillEmpty = TypeVar("PreFillEmpty")
+
 
 class CodeConfig(TypedDict):
     """
     The config of the code box.
 
     For output.
     """
```

### Comparing `funix-0.4.2/backend/funix/hint/layout.py` & `funix-0.4.3/backend/funix/hint/layout.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/prep/global_to_session.py` & `funix-0.4.3/backend/funix/prep/global_to_session.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/session/__init__.py` & `funix-0.4.3/backend/funix/session/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/test/test_magic.py` & `funix-0.4.3/backend/funix/test/test_magic.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/theme/__init__.py` & `funix-0.4.3/backend/funix/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/util/module.py` & `funix-0.4.3/backend/funix/util/module.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/util/network.py` & `funix-0.4.3/backend/funix/util/network.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/widget/__init__.py` & `funix-0.4.3/backend/funix/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix/widget/builtin.py` & `funix-0.4.3/backend/funix/widget/builtin.py`

 * *Files identical despite different names*

### Comparing `funix-0.4.2/backend/funix.egg-info/PKG-INFO` & `funix-0.4.3/backend/funix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funix
-Version: 0.4.2
+Version: 0.4.3
 Summary: Building web apps without manually creating widgets
 Author-email: "Textea Inc." <bao@textea.co>
 License: MIT License
         
         Copyright (c) 2022-2023 Textea Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funix Version: 0.4.2 Summary: Building web apps
+Metadata-Version: 2.1 Name: funix Version: 0.4.3 Summary: Building web apps
 without manually creating widgets Author-email: "Textea Inc."
 textea.co> License: MIT License Copyright (c) 2022-2023 Textea Inc. Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `funix-0.4.2/backend/funix.egg-info/SOURCES.txt` & `funix-0.4.3/backend/funix.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 backend/funix/build/asset-manifest.json
 backend/funix/build/favicon.ico
 backend/funix/build/index.html
 backend/funix/build/logo192.png
 backend/funix/build/logo512.png
 backend/funix/build/manifest.json
 backend/funix/build/static/css/main.521e60ca.css
-backend/funix/build/static/js/main.72703b71.js
-backend/funix/build/static/js/main.72703b71.js.LICENSE.txt
-backend/funix/build/static/media/pdf.worker.5036a5d54184cef29958.js
-backend/funix/build/static/media/pdf.worker.5036a5d54184cef29958.js.LICENSE.txt
+backend/funix/build/static/js/main.ef806516.js
+backend/funix/build/static/js/main.ef806516.js.LICENSE.txt
 backend/funix/config/__init__.py
 backend/funix/decorator/__init__.py
 backend/funix/decorator/file.py
 backend/funix/decorator/magic.py
 backend/funix/frontend/__init__.py
 backend/funix/hint/__init__.py
 backend/funix/hint/layout.py
```

### Comparing `funix-0.4.2/pyproject.toml` & `funix-0.4.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "funix"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   {name = "Textea Inc.", email = "bao@textea.co"}
 ]
 license = {file = "LICENSE"}
 description = "Building web apps without manually creating widgets"
 readme = "README.md"
 requires-python = ">=3.10"
```


# Comparing `tmp/gajou_cli-0.1.7.tar.gz` & `tmp/gajou_cli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gajou_cli-0.1.7.tar", last modified: Fri Jan 13 08:38:59 2023, max compression
+gzip compressed data, was "gajou_cli-0.1.8.tar", last modified: Mon Jul  3 08:07:00 2023, max compression
```

## Comparing `gajou_cli-0.1.7.tar` & `gajou_cli-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 artyomkomarenko  (1000) artyomkomarenko  (1000)        0 2023-01-13 08:38:59.182442 gajou_cli-0.1.7/
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)     1073 2022-10-06 21:55:00.000000 gajou_cli-0.1.7/LICENSE
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      759 2023-01-13 08:38:59.182442 gajou_cli-0.1.7/PKG-INFO
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      270 2022-10-07 07:57:08.000000 gajou_cli-0.1.7/README.md
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      104 2022-10-03 12:34:13.000000 gajou_cli-0.1.7/pyproject.toml
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      610 2023-01-13 08:38:59.182442 gajou_cli-0.1.7/setup.cfg
-drwxrwxr-x   0 artyomkomarenko  (1000) artyomkomarenko  (1000)        0 2023-01-13 08:38:59.182442 gajou_cli-0.1.7/src/
-drwxrwxr-x   0 artyomkomarenko  (1000) artyomkomarenko  (1000)        0 2023-01-13 08:38:59.182442 gajou_cli-0.1.7/src/gajou_cli/
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      106 2022-10-03 12:34:13.000000 gajou_cli-0.1.7/src/gajou_cli/__init__.py
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)     2405 2023-01-13 08:37:24.000000 gajou_cli-0.1.7/src/gajou_cli/base_cli.py
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      160 2022-10-03 12:34:13.000000 gajou_cli-0.1.7/src/gajou_cli/cli_response.py
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      111 2022-10-03 12:34:13.000000 gajou_cli-0.1.7/src/gajou_cli/return_codes.py
-drwxrwxr-x   0 artyomkomarenko  (1000) artyomkomarenko  (1000)        0 2023-01-13 08:38:59.182442 gajou_cli-0.1.7/src/gajou_cli.egg-info/
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      759 2023-01-13 08:38:59.000000 gajou_cli-0.1.7/src/gajou_cli.egg-info/PKG-INFO
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      302 2023-01-13 08:38:59.000000 gajou_cli-0.1.7/src/gajou_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)        1 2023-01-13 08:38:59.000000 gajou_cli-0.1.7/src/gajou_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)       10 2023-01-13 08:38:59.000000 gajou_cli-0.1.7/src/gajou_cli.egg-info/top_level.txt
+drwxrwxr-x   0 artyomkomarenko  (1000) artyomkomarenko  (1000)        0 2023-07-03 08:07:00.934688 gajou_cli-0.1.8/
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)     1073 2022-10-06 21:55:00.000000 gajou_cli-0.1.8/LICENSE
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      759 2023-07-03 08:07:00.934688 gajou_cli-0.1.8/PKG-INFO
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      270 2022-10-07 07:57:08.000000 gajou_cli-0.1.8/README.md
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      104 2022-10-03 12:34:13.000000 gajou_cli-0.1.8/pyproject.toml
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      610 2023-07-03 08:07:00.938688 gajou_cli-0.1.8/setup.cfg
+drwxrwxr-x   0 artyomkomarenko  (1000) artyomkomarenko  (1000)        0 2023-07-03 08:07:00.934688 gajou_cli-0.1.8/src/
+drwxrwxr-x   0 artyomkomarenko  (1000) artyomkomarenko  (1000)        0 2023-07-03 08:07:00.934688 gajou_cli-0.1.8/src/gajou_cli/
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      106 2022-10-03 12:34:13.000000 gajou_cli-0.1.8/src/gajou_cli/__init__.py
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)     2405 2023-01-13 08:37:24.000000 gajou_cli-0.1.8/src/gajou_cli/base_cli.py
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      160 2022-10-03 12:34:13.000000 gajou_cli-0.1.8/src/gajou_cli/cli_response.py
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      127 2023-07-03 08:05:50.000000 gajou_cli-0.1.8/src/gajou_cli/return_codes.py
+drwxrwxr-x   0 artyomkomarenko  (1000) artyomkomarenko  (1000)        0 2023-07-03 08:07:00.934688 gajou_cli-0.1.8/src/gajou_cli.egg-info/
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      759 2023-07-03 08:07:00.000000 gajou_cli-0.1.8/src/gajou_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)      302 2023-07-03 08:07:00.000000 gajou_cli-0.1.8/src/gajou_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)        1 2023-07-03 08:07:00.000000 gajou_cli-0.1.8/src/gajou_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 artyomkomarenko  (1000) artyomkomarenko  (1000)       10 2023-07-03 08:07:00.000000 gajou_cli-0.1.8/src/gajou_cli.egg-info/top_level.txt
```

### Comparing `gajou_cli-0.1.7/LICENSE` & `gajou_cli-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gajou_cli-0.1.7/PKG-INFO` & `gajou_cli-0.1.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gajou_cli
-Version: 0.1.7
+Version: 0.1.8
 Summary: Base classes and helpers to make QA autotests for CLI
 Home-page: https://github.com/ArtyomKomarenko/gajou-cli
 Author: Artyom Komarenko
 Author-email: artyom.komarenko@mail.ru
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gajou_cli-0.1.7/setup.cfg` & `gajou_cli-0.1.8/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gajou_cli
-version = 0.1.7
+version = 0.1.8
 author = Artyom Komarenko
 author_email = artyom.komarenko@mail.ru
 description = Base classes and helpers to make QA autotests for CLI
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ArtyomKomarenko/gajou-cli
 license = MIT License
```

### Comparing `gajou_cli-0.1.7/src/gajou_cli/base_cli.py` & `gajou_cli-0.1.8/src/gajou_cli/base_cli.py`

 * *Files identical despite different names*


# Comparing `tmp/lemmy_nhl-1.5.2.tar.gz` & `tmp/lemmy_nhl-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemmy_nhl-1.5.2.tar", last modified: Mon Jul  3 04:03:19 2023, max compression
+gzip compressed data, was "lemmy_nhl-1.5.3.tar", last modified: Mon Jul  3 04:10:51 2023, max compression
```

## Comparing `lemmy_nhl-1.5.2.tar` & `lemmy_nhl-1.5.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:03:19.390560 lemmy_nhl-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 04:03:05.000000 lemmy_nhl-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-03 04:03:19.390560 lemmy_nhl-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-03 04:03:05.000000 lemmy_nhl-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 04:03:05.000000 lemmy_nhl-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-03 04:03:19.390560 lemmy_nhl-1.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:03:19.386561 lemmy_nhl-1.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:03:19.390560 lemmy_nhl-1.5.2/src/lemmy_nhl/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-03 04:03:05.000000 lemmy_nhl-1.5.2/src/lemmy_nhl/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-03 04:03:05.000000 lemmy_nhl-1.5.2/src/lemmy_nhl/draft_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-07-03 04:03:05.000000 lemmy_nhl-1.5.2/src/lemmy_nhl/lemmy_nhl_bot_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-07-03 04:03:05.000000 lemmy_nhl-1.5.2/src/lemmy_nhl/post_body.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:03:19.390560 lemmy_nhl-1.5.2/src/lemmy_nhl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-03 04:03:19.000000 lemmy_nhl-1.5.2/src/lemmy_nhl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 04:03:19.000000 lemmy_nhl-1.5.2/src/lemmy_nhl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:03:19.000000 lemmy_nhl-1.5.2/src/lemmy_nhl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-03 04:03:19.000000 lemmy_nhl-1.5.2/src/lemmy_nhl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 04:03:19.000000 lemmy_nhl-1.5.2/src/lemmy_nhl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 04:03:19.000000 lemmy_nhl-1.5.2/src/lemmy_nhl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:10:51.380851 lemmy_nhl-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-03 04:10:51.380851 lemmy_nhl-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-03 04:10:51.380851 lemmy_nhl-1.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:10:51.380851 lemmy_nhl-1.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:10:51.380851 lemmy_nhl-1.5.3/src/lemmy_nhl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/src/lemmy_nhl/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/src/lemmy_nhl/draft_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/src/lemmy_nhl/lemmy_nhl_bot_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/src/lemmy_nhl/post_body.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:10:51.380851 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-03 04:10:51.000000 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 04:10:51.000000 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:10:51.000000 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-03 04:10:51.000000 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 04:10:51.000000 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 04:10:51.000000 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/top_level.txt
```

### Comparing `lemmy_nhl-1.5.2/LICENSE` & `lemmy_nhl-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lemmy_nhl-1.5.2/PKG-INFO` & `lemmy_nhl-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemmy_nhl
-Version: 1.5.2
+Version: 1.5.3
 Summary: bot to add live scores to lemmy community for hockey games
 Home-page: https://github.com/socphoenix/lemmy_nhl_bot
 Author: socphoenix
 License: Apache 2.0
 Keywords: lemmy,hockey,bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lemmy_nhl-1.5.2/README.md` & `lemmy_nhl-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `lemmy_nhl-1.5.2/setup.cfg` & `lemmy_nhl-1.5.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lemmy_nhl
-version = 1.5.2
+version = 1.5.3
 author = socphoenix
 url = https://github.com/socphoenix/lemmy_nhl_bot
 description = bot to add live scores to lemmy community for hockey games
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = lemmy, hockey, bot
 license = Apache 2.0
```

### Comparing `lemmy_nhl-1.5.2/src/lemmy_nhl/config.py` & `lemmy_nhl-1.5.3/src/lemmy_nhl/config.py`

 * *Files identical despite different names*

### Comparing `lemmy_nhl-1.5.2/src/lemmy_nhl/draft_bot.py` & `lemmy_nhl-1.5.3/src/lemmy_nhl/draft_bot.py`

 * *Files identical despite different names*

### Comparing `lemmy_nhl-1.5.2/src/lemmy_nhl/lemmy_nhl_bot_daemon.py` & `lemmy_nhl-1.5.3/src/lemmy_nhl/lemmy_nhl_bot_daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import requests
 import sqlite3
 from plemmy import LemmyHttp
 import os.path
 import time
 import sys
-import post_body
+from lemmy_nhl import post_body
 
 teamID = 0
 CID = 0
 isMod = "n"
 gameOver = False
 standings = False
 stats = False
```

### Comparing `lemmy_nhl-1.5.2/src/lemmy_nhl/post_body.py` & `lemmy_nhl-1.5.3/src/lemmy_nhl/post_body.py`

 * *Files identical despite different names*

### Comparing `lemmy_nhl-1.5.2/src/lemmy_nhl.egg-info/PKG-INFO` & `lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemmy-nhl
-Version: 1.5.2
+Version: 1.5.3
 Summary: bot to add live scores to lemmy community for hockey games
 Home-page: https://github.com/socphoenix/lemmy_nhl_bot
 Author: socphoenix
 License: Apache 2.0
 Keywords: lemmy,hockey,bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


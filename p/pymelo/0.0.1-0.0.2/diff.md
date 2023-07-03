# Comparing `tmp/pymelo-0.0.1.tar.gz` & `tmp/pymelo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymelo-0.0.1.tar", last modified: Mon Jul  3 12:40:02 2023, max compression
+gzip compressed data, was "pymelo-0.0.2.tar", last modified: Mon Jul  3 13:43:09 2023, max compression
```

## Comparing `pymelo-0.0.1.tar` & `pymelo-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 12:40:02.842134 pymelo-0.0.1/
--rw-rw-rw-   0        0        0    35149 2023-07-03 11:48:32.000000 pymelo-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1191 2023-07-03 12:40:02.840135 pymelo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      899 2023-07-03 11:48:32.000000 pymelo-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 12:40:02.837144 pymelo-0.0.1/pymelo.egg-info/
--rw-rw-rw-   0        0        0     1191 2023-07-03 12:40:02.000000 pymelo-0.0.1/pymelo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-07-03 12:40:02.000000 pymelo-0.0.1/pymelo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 12:40:02.000000 pymelo-0.0.1/pymelo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 12:40:02.000000 pymelo-0.0.1/pymelo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 12:40:02.842134 pymelo-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      434 2023-07-03 11:48:32.000000 pymelo-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:43:09.920503 pymelo-0.0.2/
+-rw-rw-rw-   0        0        0    35149 2023-07-03 11:48:32.000000 pymelo-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1191 2023-07-03 13:43:09.920503 pymelo-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      899 2023-07-03 11:48:32.000000 pymelo-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 13:43:09.902234 pymelo-0.0.2/pymelo/
+-rw-rw-rw-   0        0        0     1085 2023-07-03 13:38:14.000000 pymelo-0.0.2/pymelo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:43:09.918387 pymelo-0.0.2/pymelo.egg-info/
+-rw-rw-rw-   0        0        0     1191 2023-07-03 13:43:09.000000 pymelo-0.0.2/pymelo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2023-07-03 13:43:09.000000 pymelo-0.0.2/pymelo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 13:43:09.000000 pymelo-0.0.2/pymelo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 13:43:09.000000 pymelo-0.0.2/pymelo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 13:43:09.921489 pymelo-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      434 2023-07-03 13:37:50.000000 pymelo-0.0.2/setup.py
```

### Comparing `pymelo-0.0.1/LICENSE` & `pymelo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymelo-0.0.1/PKG-INFO` & `pymelo-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymelo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wrapper for DiscordPomeloAPI
 Home-page: https://github.com/Nemupy/pymelo
 Author: Nemupy
 Author-email: nemu.otoyume@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pymelo-0.0.1/README.md` & `pymelo-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pymelo-0.0.1/pymelo.egg-info/PKG-INFO` & `pymelo-0.0.2/pymelo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymelo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wrapper for DiscordPomeloAPI
 Home-page: https://github.com/Nemupy/pymelo
 Author: Nemupy
 Author-email: nemu.otoyume@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


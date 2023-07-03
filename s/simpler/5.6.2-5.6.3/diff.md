# Comparing `tmp/simpler-5.6.2.tar.gz` & `tmp/simpler-5.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpler-5.6.2.tar", last modified: Mon Jul  3 13:09:03 2023, max compression
+gzip compressed data, was "simpler-5.6.3.tar", last modified: Mon Jul  3 13:10:00 2023, max compression
```

## Comparing `simpler-5.6.2.tar` & `simpler-5.6.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 13:09:03.410199 simpler-5.6.2/
--rw-rw-rw-   0        0        0     1100 2020-12-02 21:28:55.000000 simpler-5.6.2/LICENSE
--rw-rw-rw-   0        0        0     1075 2023-07-03 13:09:03.409198 simpler-5.6.2/PKG-INFO
--rw-rw-rw-   0        0        0      570 2021-05-06 07:40:31.000000 simpler-5.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 13:09:03.410199 simpler-5.6.2/setup.cfg
--rw-rw-rw-   0        0        0      996 2022-05-24 11:35:04.000000 simpler-5.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 13:09:03.305166 simpler-5.6.2/simpler/
--rw-rw-rw-   0        0        0     1239 2022-10-27 23:18:07.000000 simpler-5.6.2/simpler/__init__.py
--rw-rw-rw-   0        0        0       21 2023-07-03 13:08:22.000000 simpler-5.6.2/simpler/_version.py
--rw-rw-rw-   0        0        0     2582 2022-10-26 10:50:24.000000 simpler-5.6.2/simpler/algorithms.py
--rw-rw-rw-   0        0        0     2349 2022-02-07 08:15:59.000000 simpler-5.6.2/simpler/bioinformatics.py
--rw-rw-rw-   0        0        0    17378 2023-07-03 13:07:58.000000 simpler-5.6.2/simpler/connectors.py
--rw-rw-rw-   0        0        0    16275 2022-10-28 00:02:21.000000 simpler-5.6.2/simpler/files.py
--rw-rw-rw-   0        0        0     1937 2022-02-07 08:32:41.000000 simpler-5.6.2/simpler/format.py
--rw-rw-rw-   0        0        0     1041 2022-02-07 08:33:54.000000 simpler-5.6.2/simpler/mail.py
--rw-rw-rw-   0        0        0     5015 2022-02-07 08:36:02.000000 simpler-5.6.2/simpler/math.py
--rw-rw-rw-   0        0        0     1195 2022-02-07 08:37:29.000000 simpler-5.6.2/simpler/profiling.py
--rw-rw-rw-   0        0        0     1310 2022-08-16 09:16:01.000000 simpler-5.6.2/simpler/sparql.py
--rw-rw-rw-   0        0        0     1291 2022-10-27 23:17:50.000000 simpler-5.6.2/simpler/terminal.py
--rw-rw-rw-   0        0        0     3921 2022-05-28 23:07:45.000000 simpler-5.6.2/simpler/tests.py
--rw-rw-rw-   0        0        0     3961 2023-02-07 12:04:53.000000 simpler-5.6.2/simpler/validation.py
--rw-rw-rw-   0        0        0    12956 2022-04-08 09:59:11.000000 simpler-5.6.2/simpler/web.py
-drwxrwxrwx   0        0        0        0 2023-07-03 13:09:03.407201 simpler-5.6.2/simpler.egg-info/
--rw-rw-rw-   0        0        0     1075 2023-07-03 13:09:02.000000 simpler-5.6.2/simpler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-07-03 13:09:03.000000 simpler-5.6.2/simpler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 13:09:02.000000 simpler-5.6.2/simpler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-07-03 13:09:02.000000 simpler-5.6.2/simpler.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 13:09:02.000000 simpler-5.6.2/simpler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 13:10:00.577623 simpler-5.6.3/
+-rw-rw-rw-   0        0        0     1100 2020-12-02 21:28:55.000000 simpler-5.6.3/LICENSE
+-rw-rw-rw-   0        0        0     1075 2023-07-03 13:10:00.577623 simpler-5.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2021-05-06 07:40:31.000000 simpler-5.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 13:10:00.577623 simpler-5.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      996 2022-05-24 11:35:04.000000 simpler-5.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:10:00.561999 simpler-5.6.3/simpler/
+-rw-rw-rw-   0        0        0     1239 2022-10-27 23:18:07.000000 simpler-5.6.3/simpler/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-07-03 13:09:46.000000 simpler-5.6.3/simpler/_version.py
+-rw-rw-rw-   0        0        0     2582 2022-10-26 10:50:24.000000 simpler-5.6.3/simpler/algorithms.py
+-rw-rw-rw-   0        0        0     2349 2022-02-07 08:15:59.000000 simpler-5.6.3/simpler/bioinformatics.py
+-rw-rw-rw-   0        0        0    17378 2023-07-03 13:07:58.000000 simpler-5.6.3/simpler/connectors.py
+-rw-rw-rw-   0        0        0    16275 2022-10-28 00:02:21.000000 simpler-5.6.3/simpler/files.py
+-rw-rw-rw-   0        0        0     1937 2022-02-07 08:32:41.000000 simpler-5.6.3/simpler/format.py
+-rw-rw-rw-   0        0        0     1041 2022-02-07 08:33:54.000000 simpler-5.6.3/simpler/mail.py
+-rw-rw-rw-   0        0        0     5015 2022-02-07 08:36:02.000000 simpler-5.6.3/simpler/math.py
+-rw-rw-rw-   0        0        0     1195 2022-02-07 08:37:29.000000 simpler-5.6.3/simpler/profiling.py
+-rw-rw-rw-   0        0        0     1310 2022-08-16 09:16:01.000000 simpler-5.6.3/simpler/sparql.py
+-rw-rw-rw-   0        0        0     1291 2022-10-27 23:17:50.000000 simpler-5.6.3/simpler/terminal.py
+-rw-rw-rw-   0        0        0     3921 2022-05-28 23:07:45.000000 simpler-5.6.3/simpler/tests.py
+-rw-rw-rw-   0        0        0     3961 2023-02-07 12:04:53.000000 simpler-5.6.3/simpler/validation.py
+-rw-rw-rw-   0        0        0    12956 2022-04-08 09:59:11.000000 simpler-5.6.3/simpler/web.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:10:00.577623 simpler-5.6.3/simpler.egg-info/
+-rw-rw-rw-   0        0        0     1075 2023-07-03 13:09:59.000000 simpler-5.6.3/simpler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-07-03 13:10:00.000000 simpler-5.6.3/simpler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 13:10:00.000000 simpler-5.6.3/simpler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-07-03 13:10:00.000000 simpler-5.6.3/simpler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 13:10:00.000000 simpler-5.6.3/simpler.egg-info/top_level.txt
```

### Comparing `simpler-5.6.2/LICENSE` & `simpler-5.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/PKG-INFO` & `simpler-5.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpler
-Version: 5.6.2
+Version: 5.6.3
 Summary: Makes Python simpler.
 Home-page: https://github.com/juancroldan/simpler
 Author: Juan C. Roldán
 Author-email: juancarlos@sevilla.es
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `simpler-5.6.2/README.md` & `simpler-5.6.3/README.md`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/setup.py` & `simpler-5.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/__init__.py` & `simpler-5.6.3/simpler/__init__.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/algorithms.py` & `simpler-5.6.3/simpler/algorithms.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/bioinformatics.py` & `simpler-5.6.3/simpler/bioinformatics.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/connectors.py` & `simpler-5.6.3/simpler/connectors.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/files.py` & `simpler-5.6.3/simpler/files.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/format.py` & `simpler-5.6.3/simpler/format.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/mail.py` & `simpler-5.6.3/simpler/mail.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/math.py` & `simpler-5.6.3/simpler/math.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/profiling.py` & `simpler-5.6.3/simpler/profiling.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/sparql.py` & `simpler-5.6.3/simpler/sparql.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/terminal.py` & `simpler-5.6.3/simpler/terminal.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/tests.py` & `simpler-5.6.3/simpler/tests.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/validation.py` & `simpler-5.6.3/simpler/validation.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler/web.py` & `simpler-5.6.3/simpler/web.py`

 * *Files identical despite different names*

### Comparing `simpler-5.6.2/simpler.egg-info/PKG-INFO` & `simpler-5.6.3/simpler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpler
-Version: 5.6.2
+Version: 5.6.3
 Summary: Makes Python simpler.
 Home-page: https://github.com/juancroldan/simpler
 Author: Juan C. Roldán
 Author-email: juancarlos@sevilla.es
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```


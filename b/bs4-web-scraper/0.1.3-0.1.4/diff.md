# Comparing `tmp/bs4_web_scraper-0.1.3.tar.gz` & `tmp/bs4_web_scraper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs4_web_scraper-0.1.3.tar", last modified: Sun Jun  4 14:34:29 2023, max compression
+gzip compressed data, was "bs4_web_scraper-0.1.4.tar", last modified: Mon Jul  3 17:17:30 2023, max compression
```

## Comparing `bs4_web_scraper-0.1.3.tar` & `bs4_web_scraper-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 14:34:29.141370 bs4_web_scraper-0.1.3/
--rw-rw-rw-   0        0        0     1104 2023-03-07 14:14:59.000000 bs4_web_scraper-0.1.3/LICENSE.md
--rw-rw-rw-   0        0        0    19798 2023-06-04 14:34:29.141370 bs4_web_scraper-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    18458 2023-05-28 18:46:31.000000 bs4_web_scraper-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 14:34:29.013367 bs4_web_scraper-0.1.3/bs4_web_scraper/
--rw-rw-rw-   0        0        0     3635 2023-05-28 18:48:55.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/__init__.py
--rw-rw-rw-   0        0        0    44567 2023-05-31 20:43:03.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/base.py
--rw-rw-rw-   0        0        0     2102 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/exceptions.py
--rw-rw-rw-   0        0        0    13603 2023-06-04 13:45:20.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/file_handler.py
--rw-rw-rw-   0        0        0     5642 2023-05-27 10:03:10.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/logger.py
--rw-rw-rw-   0        0        0     4864 2023-06-01 03:31:13.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/request_limiter.py
--rw-rw-rw-   0        0        0    44240 2023-06-02 17:56:05.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/scraper.py
--rw-rw-rw-   0        0        0    23599 2023-06-04 14:12:14.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/translate.py
--rw-rw-rw-   0        0        0     3906 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 14:34:29.109377 bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/
--rw-rw-rw-   0        0        0    19798 2023-06-04 14:34:28.000000 bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-06-04 14:34:28.000000 bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 14:34:28.000000 bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2023-06-04 14:34:28.000000 bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-04 14:34:28.000000 bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1731 2023-06-04 14:32:54.000000 bs4_web_scraper-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 14:34:29.149369 bs4_web_scraper-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-04 14:34:29.141370 bs4_web_scraper-0.1.3/tests/
--rw-rw-rw-   0        0        0    10390 2023-06-03 23:28:03.000000 bs4_web_scraper-0.1.3/tests/test_base.py
--rw-rw-rw-   0        0        0     9022 2023-06-04 11:38:04.000000 bs4_web_scraper-0.1.3/tests/test_file_handler.py
--rw-rw-rw-   0        0        0     9088 2023-06-02 18:09:58.000000 bs4_web_scraper-0.1.3/tests/test_scraper.py
--rw-rw-rw-   0        0        0     3938 2023-06-04 14:15:02.000000 bs4_web_scraper-0.1.3/tests/test_translate.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:17:30.305391 bs4_web_scraper-0.1.4/
+-rw-rw-rw-   0        0        0     1104 2023-03-07 14:14:59.000000 bs4_web_scraper-0.1.4/LICENSE.md
+-rw-rw-rw-   0        0        0    19796 2023-07-03 17:17:30.305391 bs4_web_scraper-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    18458 2023-05-28 18:46:31.000000 bs4_web_scraper-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 17:17:29.899536 bs4_web_scraper-0.1.4/bs4_web_scraper/
+-rw-rw-rw-   0        0        0     3635 2023-05-28 18:48:55.000000 bs4_web_scraper-0.1.4/bs4_web_scraper/__init__.py
+-rw-rw-rw-   0        0        0    44567 2023-05-31 20:43:03.000000 bs4_web_scraper-0.1.4/bs4_web_scraper/base.py
+-rw-rw-rw-   0        0        0     2102 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.4/bs4_web_scraper/exceptions.py
+-rw-rw-rw-   0        0        0    13603 2023-06-04 13:45:20.000000 bs4_web_scraper-0.1.4/bs4_web_scraper/file_handler.py
+-rw-rw-rw-   0        0        0     5642 2023-05-27 10:03:10.000000 bs4_web_scraper-0.1.4/bs4_web_scraper/logger.py
+-rw-rw-rw-   0        0        0     4864 2023-06-01 03:31:13.000000 bs4_web_scraper-0.1.4/bs4_web_scraper/request_limiter.py
+-rw-rw-rw-   0        0        0    44240 2023-06-02 17:56:05.000000 bs4_web_scraper-0.1.4/bs4_web_scraper/scraper.py
+-rw-rw-rw-   0        0        0    23599 2023-06-04 14:12:14.000000 bs4_web_scraper-0.1.4/bs4_web_scraper/translate.py
+-rw-rw-rw-   0        0        0     3906 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.4/bs4_web_scraper/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:17:30.116788 bs4_web_scraper-0.1.4/bs4_web_scraper.egg-info/
+-rw-rw-rw-   0        0        0    19796 2023-07-03 17:17:28.000000 bs4_web_scraper-0.1.4/bs4_web_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-07-03 17:17:28.000000 bs4_web_scraper-0.1.4/bs4_web_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 17:17:28.000000 bs4_web_scraper-0.1.4/bs4_web_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-07-03 17:17:28.000000 bs4_web_scraper-0.1.4/bs4_web_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-03 17:17:28.000000 bs4_web_scraper-0.1.4/bs4_web_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1729 2023-07-03 17:16:24.000000 bs4_web_scraper-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 17:17:30.305391 bs4_web_scraper-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 17:17:30.280902 bs4_web_scraper-0.1.4/tests/
+-rw-rw-rw-   0        0        0    10390 2023-06-03 23:28:03.000000 bs4_web_scraper-0.1.4/tests/test_base.py
+-rw-rw-rw-   0        0        0     9022 2023-06-04 11:38:04.000000 bs4_web_scraper-0.1.4/tests/test_file_handler.py
+-rw-rw-rw-   0        0        0     9088 2023-06-02 18:09:58.000000 bs4_web_scraper-0.1.4/tests/test_scraper.py
+-rw-rw-rw-   0        0        0     3938 2023-06-04 14:15:02.000000 bs4_web_scraper-0.1.4/tests/test_translate.py
```

### Comparing `bs4_web_scraper-0.1.3/LICENSE.md` & `bs4_web_scraper-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/PKG-INFO` & `bs4_web_scraper-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: bs4_web_scraper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A web scraper based on the BeautifulSoup4 library and translators package.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/bs4_web_scraper
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/bs4_web_scraper/issues
 Project-URL: Repository, https://github.com/ti-oluwa/bs4_web_scraper
 Keywords: web scraper,bs4,beautifulsoup4,web scraping,web scraping with python,web scraping with bs4,web scraping with beautifulsoup4,web scraping with translation,web scraping with translation to other languages,web scraping with translation to other languages with python,web scraping with translation to other languages with bs4,web scraping with translation to other languages with beautifulsoup4,web scraping with translation to other languages with python and bs4,web scraping with translation to other languages with python and beautifulsoup4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ## bs4_web_scraper
 
 ### __A web scraper based on the BeautifulSoup4 library with translation capabilities.__
```

### Comparing `bs4_web_scraper-0.1.3/README.md` & `bs4_web_scraper-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/bs4_web_scraper/__init__.py` & `bs4_web_scraper-0.1.4/bs4_web_scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/bs4_web_scraper/base.py` & `bs4_web_scraper-0.1.4/bs4_web_scraper/base.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/bs4_web_scraper/exceptions.py` & `bs4_web_scraper-0.1.4/bs4_web_scraper/exceptions.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/bs4_web_scraper/file_handler.py` & `bs4_web_scraper-0.1.4/bs4_web_scraper/file_handler.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/bs4_web_scraper/logger.py` & `bs4_web_scraper-0.1.4/bs4_web_scraper/logger.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/bs4_web_scraper/request_limiter.py` & `bs4_web_scraper-0.1.4/bs4_web_scraper/request_limiter.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/bs4_web_scraper/scraper.py` & `bs4_web_scraper-0.1.4/bs4_web_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/bs4_web_scraper/translate.py` & `bs4_web_scraper-0.1.4/bs4_web_scraper/translate.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/bs4_web_scraper/utils.py` & `bs4_web_scraper-0.1.4/bs4_web_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/PKG-INFO` & `bs4_web_scraper-0.1.4/bs4_web_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: bs4-web-scraper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A web scraper based on the BeautifulSoup4 library and translators package.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/bs4_web_scraper
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/bs4_web_scraper/issues
 Project-URL: Repository, https://github.com/ti-oluwa/bs4_web_scraper
 Keywords: web scraper,bs4,beautifulsoup4,web scraping,web scraping with python,web scraping with bs4,web scraping with beautifulsoup4,web scraping with translation,web scraping with translation to other languages,web scraping with translation to other languages with python,web scraping with translation to other languages with bs4,web scraping with translation to other languages with beautifulsoup4,web scraping with translation to other languages with python and bs4,web scraping with translation to other languages with python and beautifulsoup4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ## bs4_web_scraper
 
 ### __A web scraper based on the BeautifulSoup4 library with translation capabilities.__
```

### Comparing `bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/SOURCES.txt` & `bs4_web_scraper-0.1.4/bs4_web_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/pyproject.toml` & `bs4_web_scraper-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bs4_web_scraper"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 maintainers = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 description = "A web scraper based on the BeautifulSoup4 library and translators package."
@@ -18,20 +18,20 @@
     'web scraping with beautifulsoup4', 'web scraping with translation', 
     'web scraping with translation to other languages', 
     'web scraping with translation to other languages with python', 'web scraping with translation to other languages with bs4', 
     'web scraping with translation to other languages with beautifulsoup4', 'web scraping with translation to other languages with python and bs4', 
     'web scraping with translation to other languages with python and beautifulsoup4',
 ]
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Environment :: Console",
 ]
 dependencies = [
     'beautifulsoup4>=4.11.2',
     'lxml>=4.9.2',
     'requests>=2.28.1',
     'html5lib>=1.1',
```

### Comparing `bs4_web_scraper-0.1.3/tests/test_base.py` & `bs4_web_scraper-0.1.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/tests/test_file_handler.py` & `bs4_web_scraper-0.1.4/tests/test_file_handler.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/tests/test_scraper.py` & `bs4_web_scraper-0.1.4/tests/test_scraper.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.3/tests/test_translate.py` & `bs4_web_scraper-0.1.4/tests/test_translate.py`

 * *Files identical despite different names*


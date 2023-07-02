# Comparing `tmp/eparse-0.6.1.tar.gz` & `tmp/eparse-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eparse-0.6.1.tar", last modified: Thu Jun 22 18:58:31 2023, max compression
+gzip compressed data, was "eparse-0.6.2.tar", last modified: Sun Jul  2 23:51:28 2023, max compression
```

## Comparing `eparse-0.6.1.tar` & `eparse-0.6.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-22 18:58:31.265839 eparse-0.6.1/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.6.1/AUTHORS.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.6.1/CONTRIBUTING.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      681 2023-06-22 18:56:31.000000 eparse-0.6.1/HISTORY.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.6.1/LICENSE
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.6.1/MANIFEST.in
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    13049 2023-06-22 18:58:31.265839 eparse-0.6.1/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    11620 2023-06-16 03:28:39.000000 eparse-0.6.1/README.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-22 18:58:31.265839 eparse-0.6.1/docs/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/Makefile
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/authors.rst
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/conf.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/contributing.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/history.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/index.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/installation.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/make.bat
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/readme.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.6.1/docs/usage.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-22 18:58:31.265839 eparse-0.6.1/eparse/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-22 18:51:50.000000 eparse-0.6.1/eparse/__init__.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9581 2023-06-15 01:18:10.000000 eparse-0.6.1/eparse/cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     5771 2023-06-15 01:08:49.000000 eparse-0.6.1/eparse/core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     6316 2023-06-14 18:30:00.000000 eparse-0.6.1/eparse/interfaces.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.6.1/eparse/migrations.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-22 18:58:31.265839 eparse-0.6.1/eparse.egg-info/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    13049 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/SOURCES.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/dependency_links.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/entry_points.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/not-zip-safe
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/requires.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-22 18:58:31.000000 eparse-0.6.1/eparse.egg-info/top_level.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      141 2023-06-22 18:58:31.275839 eparse-0.6.1/setup.cfg
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1570 2023-06-22 18:51:42.000000 eparse-0.6.1/setup.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-22 18:58:31.265839 eparse-0.6.1/tests/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.6.1/tests/__init__.py
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.6.1/tests/eparse_unit_test_data.xlsx
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      891 2023-06-14 18:22:40.000000 eparse-0.6.1/tests/fixtures.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.6.1/tests/test.db
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1980 2023-06-14 18:22:40.000000 eparse-0.6.1/tests/test_cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-06-13 20:47:22.000000 eparse-0.6.1/tests/test_core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.6.1/tests/test_interfaces.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-02 23:51:28.647887 eparse-0.6.2/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.6.2/AUTHORS.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.6.2/CONTRIBUTING.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      681 2023-06-22 18:56:31.000000 eparse-0.6.2/HISTORY.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.6.2/LICENSE
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.6.2/MANIFEST.in
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    13150 2023-07-02 23:51:28.647887 eparse-0.6.2/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    11620 2023-06-16 03:28:39.000000 eparse-0.6.2/README.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-02 23:51:28.637887 eparse-0.6.2/docs/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/Makefile
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/authors.rst
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/conf.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/contributing.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/history.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/index.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/installation.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/make.bat
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/readme.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.6.2/docs/usage.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-02 23:51:28.637887 eparse-0.6.2/eparse/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-07-02 23:50:14.000000 eparse-0.6.2/eparse/__init__.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9581 2023-06-15 01:18:10.000000 eparse-0.6.2/eparse/cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     5771 2023-07-02 23:45:12.000000 eparse-0.6.2/eparse/core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     6316 2023-06-14 18:30:00.000000 eparse-0.6.2/eparse/interfaces.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.6.2/eparse/migrations.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-02 23:51:28.637887 eparse-0.6.2/eparse.egg-info/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    13150 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      701 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/SOURCES.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/dependency_links.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/entry_points.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/not-zip-safe
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/requires.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-07-02 23:51:28.000000 eparse-0.6.2/eparse.egg-info/top_level.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      141 2023-07-02 23:51:28.647887 eparse-0.6.2/setup.cfg
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1698 2023-07-02 23:49:16.000000 eparse-0.6.2/setup.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-07-02 23:51:28.647887 eparse-0.6.2/tests/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.6.2/tests/__init__.py
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.6.2/tests/eparse_unit_test_data.xlsx
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      891 2023-06-14 18:22:40.000000 eparse-0.6.2/tests/fixtures.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)   237568 2023-06-14 14:02:00.000000 eparse-0.6.2/tests/test.db
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1980 2023-06-14 18:22:40.000000 eparse-0.6.2/tests/test_cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-07-02 23:45:12.000000 eparse-0.6.2/tests/test_core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2609 2023-06-14 13:42:33.000000 eparse-0.6.2/tests/test_interfaces.py
```

### Comparing `eparse-0.6.1/CONTRIBUTING.rst` & `eparse-0.6.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/HISTORY.rst` & `eparse-0.6.2/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/LICENSE` & `eparse-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/PKG-INFO` & `eparse-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.6.1
+Version: 0.6.2
 Summary: Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ======
 eparse
 ======
```

### Comparing `eparse-0.6.1/README.rst` & `eparse-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/docs/Makefile` & `eparse-0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/docs/conf.py` & `eparse-0.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/docs/installation.rst` & `eparse-0.6.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/docs/make.bat` & `eparse-0.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/eparse/cli.py` & `eparse-0.6.2/eparse/cli.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/eparse/core.py` & `eparse-0.6.2/eparse/core.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/eparse/interfaces.py` & `eparse-0.6.2/eparse/interfaces.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/eparse/migrations.py` & `eparse-0.6.2/eparse/migrations.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/eparse.egg-info/PKG-INFO` & `eparse-0.6.2/eparse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.6.1
+Version: 0.6.2
 Summary: Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ======
 eparse
 ======
```

### Comparing `eparse-0.6.1/eparse.egg-info/SOURCES.txt` & `eparse-0.6.2/eparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/setup.py` & `eparse-0.6.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,33 +17,37 @@
     'click>=8.0.0',
     'openpyxl>=3.0.0',
     'pandas>=2.0.0',
     'peewee>=3.16.0',
 ]
 
 test_requirements = [
+    'black',
+    'coverage',
     'flake8',
     'ipython',
     'pytest',
     'tox',
 ]
 
 setup(
     author='Chris Pappalardo',
     author_email='cpappala@gmail.com',
-    python_requires='>=3.9',
+    python_requires='>=3.8',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     description='''
     Excel spreadsheet crawler and table parser for data discovery, extraction, and querying
     ''',
     entry_points={
         'console_scripts': [
             'eparse=eparse.cli:entry_point',
@@ -55,10 +59,10 @@
     include_package_data=True,
     keywords='eparse',
     name='eparse',
     packages=find_packages(include=['eparse', 'eparse.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ChrisPappalardo/eparse',
-    version='0.6.1',
+    version='0.6.2',
     zip_safe=False,
 )
```

### Comparing `eparse-0.6.1/tests/eparse_unit_test_data.xlsx` & `eparse-0.6.2/tests/eparse_unit_test_data.xlsx`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/tests/fixtures.py` & `eparse-0.6.2/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/tests/test.db` & `eparse-0.6.2/tests/test.db`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/tests/test_cli.py` & `eparse-0.6.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/tests/test_core.py` & `eparse-0.6.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `eparse-0.6.1/tests/test_interfaces.py` & `eparse-0.6.2/tests/test_interfaces.py`

 * *Files identical despite different names*


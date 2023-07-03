# Comparing `tmp/transientNamer-0.4.5.tar.gz` & `tmp/transientNamer-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transientNamer-0.4.5.tar", last modified: Tue Jan 10 17:27:42 2023, max compression
+gzip compressed data, was "transientNamer-0.4.6.tar", last modified: Mon Jul  3 14:31:39 2023, max compression
```

## Comparing `transientNamer-0.4.5.tar` & `transientNamer-0.4.6.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 Dave       (503) staff       (20)        0 2023-01-10 17:27:42.716816 transientNamer-0.4.5/
--rw-r--r--   0 Dave       (503) staff       (20)      413 2020-05-22 17:08:33.000000 transientNamer-0.4.5/.readthedocs.yaml
--rw-r--r--   0 Dave       (503) staff       (20)     1149 2023-01-10 17:27:26.000000 transientNamer-0.4.5/CHANGES.md
--rw-r--r--   0 Dave       (503) staff       (20)    35149 2020-05-22 17:08:33.000000 transientNamer-0.4.5/LICENSE
--rw-r--r--   0 Dave       (503) staff       (20)      369 2023-01-10 16:21:07.000000 transientNamer-0.4.5/MANIFEST.in
--rw-r--r--   0 Dave       (503) staff       (20)     2506 2023-01-10 17:27:42.716568 transientNamer-0.4.5/PKG-INFO
--rw-r--r--   0 Dave       (503) staff       (20)     1906 2021-01-25 14:40:36.000000 transientNamer-0.4.5/README.md
--rw-r--r--   0 Dave       (503) staff       (20)       38 2023-01-10 17:27:42.716904 transientNamer-0.4.5/setup.cfg
--rw-r--r--   0 Dave       (503) staff       (20)     1885 2023-01-10 16:21:07.000000 transientNamer-0.4.5/setup.py
-drwxr-xr-x   0 Dave       (503) staff       (20)        0 2023-01-10 17:27:42.713149 transientNamer-0.4.5/transientNamer/
--rw-r--r--   0 Dave       (503) staff       (20)     6148 2022-11-03 17:42:31.000000 transientNamer-0.4.5/transientNamer/.DS_Store
--rw-r--r--   0 Dave       (503) staff       (20)      181 2021-01-25 14:40:36.000000 transientNamer-0.4.5/transientNamer/__init__.py
--rw-r--r--   0 Dave       (503) staff       (20)       22 2023-01-10 17:27:26.000000 transientNamer-0.4.5/transientNamer/__version__.py
--rw-r--r--   0 Dave       (503) staff       (20)    20254 2021-05-20 11:37:19.000000 transientNamer-0.4.5/transientNamer/astronotes.py
--rw-r--r--   0 Dave       (503) staff       (20)     8852 2021-05-21 07:28:11.000000 transientNamer-0.4.5/transientNamer/cl_utils.py
-drwxr-xr-x   0 Dave       (503) staff       (20)        0 2023-01-10 17:27:42.716159 transientNamer-0.4.5/transientNamer/commonutils/
--rw-r--r--   0 Dave       (503) staff       (20)      129 2020-05-22 17:08:33.000000 transientNamer-0.4.5/transientNamer/commonutils/__init__.py
--rw-r--r--   0 Dave       (503) staff       (20)      327 2020-05-22 17:08:33.000000 transientNamer-0.4.5/transientNamer/commonutils/getpackagepath.py
--rw-r--r--   0 Dave       (503) staff       (20)     2218 2021-05-20 14:59:58.000000 transientNamer-0.4.5/transientNamer/default_settings.yaml
--rw-r--r--   0 Dave       (503) staff       (20)    52991 2023-01-10 16:21:07.000000 transientNamer-0.4.5/transientNamer/search.py
--rw-r--r--   0 Dave       (503) staff       (20)     2130 2021-05-20 16:55:06.000000 transientNamer-0.4.5/transientNamer/test_settings.yaml
--rw-r--r--   0 Dave       (503) staff       (20)     3390 2020-05-22 17:08:33.000000 transientNamer-0.4.5/transientNamer/utKit.py
-drwxr-xr-x   0 Dave       (503) staff       (20)        0 2023-01-10 17:27:42.715592 transientNamer-0.4.5/transientNamer.egg-info/
--rw-r--r--   0 Dave       (503) staff       (20)     2506 2023-01-10 17:27:42.000000 transientNamer-0.4.5/transientNamer.egg-info/PKG-INFO
--rw-r--r--   0 Dave       (503) staff       (20)      676 2023-01-10 17:27:42.000000 transientNamer-0.4.5/transientNamer.egg-info/SOURCES.txt
--rw-r--r--   0 Dave       (503) staff       (20)        1 2023-01-10 17:27:42.000000 transientNamer-0.4.5/transientNamer.egg-info/dependency_links.txt
--rw-r--r--   0 Dave       (503) staff       (20)       64 2023-01-10 17:27:42.000000 transientNamer-0.4.5/transientNamer.egg-info/entry_points.txt
--rw-r--r--   0 Dave       (503) staff       (20)        1 2016-10-19 19:28:27.000000 transientNamer-0.4.5/transientNamer.egg-info/not-zip-safe
--rw-r--r--   0 Dave       (503) staff       (20)      111 2023-01-10 17:27:42.000000 transientNamer-0.4.5/transientNamer.egg-info/requires.txt
--rw-r--r--   0 Dave       (503) staff       (20)       15 2023-01-10 17:27:42.000000 transientNamer-0.4.5/transientNamer.egg-info/top_level.txt
+drwxr-xr-x   0 Dave       (503) staff       (20)        0 2023-07-03 14:31:39.145558 transientNamer-0.4.6/
+-rw-r--r--   0 Dave       (503) staff       (20)      413 2020-05-22 17:08:33.000000 transientNamer-0.4.6/.readthedocs.yaml
+-rw-r--r--   0 Dave       (503) staff       (20)     1216 2023-07-03 14:31:11.000000 transientNamer-0.4.6/CHANGES.md
+-rw-r--r--   0 Dave       (503) staff       (20)    35149 2020-05-22 17:08:33.000000 transientNamer-0.4.6/LICENSE
+-rw-r--r--   0 Dave       (503) staff       (20)      369 2023-01-10 16:21:07.000000 transientNamer-0.4.6/MANIFEST.in
+-rw-r--r--   0 Dave       (503) staff       (20)     2963 2023-07-03 14:31:39.145246 transientNamer-0.4.6/PKG-INFO
+-rw-r--r--   0 Dave       (503) staff       (20)     2363 2023-06-15 08:13:33.000000 transientNamer-0.4.6/README.md
+-rw-r--r--   0 Dave       (503) staff       (20)       38 2023-07-03 14:31:39.145683 transientNamer-0.4.6/setup.cfg
+-rw-r--r--   0 Dave       (503) staff       (20)     1885 2023-01-10 16:21:07.000000 transientNamer-0.4.6/setup.py
+drwxr-xr-x   0 Dave       (503) staff       (20)        0 2023-07-03 14:31:39.139380 transientNamer-0.4.6/transientNamer/
+-rw-r--r--   0 Dave       (503) staff       (20)     6148 2023-06-14 10:50:14.000000 transientNamer-0.4.6/transientNamer/.DS_Store
+-rw-r--r--   0 Dave       (503) staff       (20)      181 2021-01-25 14:40:36.000000 transientNamer-0.4.6/transientNamer/__init__.py
+-rw-r--r--   0 Dave       (503) staff       (20)       22 2023-07-03 14:31:11.000000 transientNamer-0.4.6/transientNamer/__version__.py
+-rw-r--r--   0 Dave       (503) staff       (20)    20252 2023-07-03 14:31:11.000000 transientNamer-0.4.6/transientNamer/astronotes.py
+-rw-r--r--   0 Dave       (503) staff       (20)     8852 2021-05-21 07:28:11.000000 transientNamer-0.4.6/transientNamer/cl_utils.py
+drwxr-xr-x   0 Dave       (503) staff       (20)        0 2023-07-03 14:31:39.144101 transientNamer-0.4.6/transientNamer/commonutils/
+-rw-r--r--   0 Dave       (503) staff       (20)      129 2020-05-22 17:08:33.000000 transientNamer-0.4.6/transientNamer/commonutils/__init__.py
+-rw-r--r--   0 Dave       (503) staff       (20)      327 2020-05-22 17:08:33.000000 transientNamer-0.4.6/transientNamer/commonutils/getpackagepath.py
+-rw-r--r--   0 Dave       (503) staff       (20)     2218 2021-05-20 14:59:58.000000 transientNamer-0.4.6/transientNamer/default_settings.yaml
+drwxr-xr-x   0 Dave       (503) staff       (20)        0 2023-07-03 14:31:39.144476 transientNamer-0.4.6/transientNamer/resources/
+-rw-r--r--   0 Dave       (503) staff       (20)     6290 2023-06-15 08:13:33.000000 transientNamer-0.4.6/transientNamer/resources/package.mplstyle
+-rw-r--r--   0 Dave       (503) staff       (20)    52991 2023-01-10 16:21:07.000000 transientNamer-0.4.6/transientNamer/search.py
+-rw-r--r--   0 Dave       (503) staff       (20)     2130 2021-05-20 16:55:06.000000 transientNamer-0.4.6/transientNamer/test_settings.yaml
+-rw-r--r--   0 Dave       (503) staff       (20)     3390 2020-05-22 17:08:33.000000 transientNamer-0.4.6/transientNamer/utKit.py
+drwxr-xr-x   0 Dave       (503) staff       (20)        0 2023-07-03 14:31:39.143340 transientNamer-0.4.6/transientNamer.egg-info/
+-rw-r--r--   0 Dave       (503) staff       (20)     2963 2023-07-03 14:31:38.000000 transientNamer-0.4.6/transientNamer.egg-info/PKG-INFO
+-rw-r--r--   0 Dave       (503) staff       (20)      718 2023-07-03 14:31:39.000000 transientNamer-0.4.6/transientNamer.egg-info/SOURCES.txt
+-rw-r--r--   0 Dave       (503) staff       (20)        1 2023-07-03 14:31:38.000000 transientNamer-0.4.6/transientNamer.egg-info/dependency_links.txt
+-rw-r--r--   0 Dave       (503) staff       (20)       64 2023-07-03 14:31:38.000000 transientNamer-0.4.6/transientNamer.egg-info/entry_points.txt
+-rw-r--r--   0 Dave       (503) staff       (20)        1 2016-10-19 19:28:27.000000 transientNamer-0.4.6/transientNamer.egg-info/not-zip-safe
+-rw-r--r--   0 Dave       (503) staff       (20)      111 2023-07-03 14:31:38.000000 transientNamer-0.4.6/transientNamer.egg-info/requires.txt
+-rw-r--r--   0 Dave       (503) staff       (20)       15 2023-07-03 14:31:38.000000 transientNamer-0.4.6/transientNamer.egg-info/top_level.txt
```

### Comparing `transientNamer-0.4.5/CHANGES.md` & `transientNamer-0.4.6/CHANGES.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 
 ## Release Notes
 
+**v0.4.6 - July 3, 2023**
+
+* **FIXED**: small fixes to unit-tests
+
 **v0.4.5 - January 10, 2023**
 
 * **FIXED**: changes to search url to reflectv changes made on the TNS. All transients should now be reported again.
 
 **v0.4.4 - June 17, 2022**
 
 * **FIXED**: unit-tests failing due to throttling from TNS
```

### Comparing `transientNamer-0.4.5/LICENSE` & `transientNamer-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `transientNamer-0.4.5/PKG-INFO` & `transientNamer-0.4.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: transientNamer
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python API for reading and caching TNS reports
 Home-page: https://github.com/thespacedoctor/transientNamer
-Download-URL: https://github.com/thespacedoctor/transientNamer/archive/v0.4.5.zip
+Download-URL: https://github.com/thespacedoctor/transientNamer/archive/v0.4.6.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: MIT
 Keywords: astronomy, transients
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # transientNamer
 
+
+
+[![](https://zenodo.org/badge/53676687.svg)](https://zenodo.org/badge/latestdoi/53676687) 
+
+
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/transientNamer)](https://pypi.org/project/transientNamer/)  
 [![](https://img.shields.io/pypi/v/transientNamer)](https://pypi.org/project/transientNamer/)  
 [![](https://img.shields.io/github/license/thespacedoctor/transientNamer)](https://github.com/thespacedoctor/transientNamer)  
 [![](https://img.shields.io/pypi/dm/transientNamer)](https://pypi.org/project/transientNamer/)  
 
@@ -36,9 +41,23 @@
 
 Documentation for transientNamer is hosted by [Read the Docs](https://transientNamer.readthedocs.io/en/master/) ([development version](https://transientNamer.readthedocs.io/en/develop/) and [master version](https://transientNamer.readthedocs.io/en/master/)). The code lives on [github](https://github.com/thespacedoctor/transientNamer). Please report any issues you find [here](https://github.com/thespacedoctor/transientNamer/issues).
 
 ## Features
 
 * 
 
+## How to cite transientNamer
+
+If you use `transientNamer` in your work, please cite using the following BibTeX entry: 
+
+```bibtex
+@software{Young_transientNamer,
+    author = {Young, David R.},
+    doi = {10.5281/zenodo.7970680},
+    license = {GPL-3.0-only},
+    title = {{transientNamer}},
+    url = {https://github.com/thespacedoctor/transientNamer}
+}
+```
+
```

### Comparing `transientNamer-0.4.5/README.md` & `transientNamer-0.4.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # transientNamer
 
+
+
+[![](https://zenodo.org/badge/53676687.svg)](https://zenodo.org/badge/latestdoi/53676687) 
+
+
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/transientNamer)](https://pypi.org/project/transientNamer/)  
 [![](https://img.shields.io/pypi/v/transientNamer)](https://pypi.org/project/transientNamer/)  
 [![](https://img.shields.io/github/license/thespacedoctor/transientNamer)](https://github.com/thespacedoctor/transientNamer)  
 [![](https://img.shields.io/pypi/dm/transientNamer)](https://pypi.org/project/transientNamer/)  
 
@@ -19,9 +24,23 @@
 
 Documentation for transientNamer is hosted by [Read the Docs](https://transientNamer.readthedocs.io/en/master/) ([development version](https://transientNamer.readthedocs.io/en/develop/) and [master version](https://transientNamer.readthedocs.io/en/master/)). The code lives on [github](https://github.com/thespacedoctor/transientNamer). Please report any issues you find [here](https://github.com/thespacedoctor/transientNamer/issues).
 
 ## Features
 
 * 
 
+## How to cite transientNamer
+
+If you use `transientNamer` in your work, please cite using the following BibTeX entry: 
+
+```bibtex
+@software{Young_transientNamer,
+    author = {Young, David R.},
+    doi = {10.5281/zenodo.7970680},
+    license = {GPL-3.0-only},
+    title = {{transientNamer}},
+    url = {https://github.com/thespacedoctor/transientNamer}
+}
+```
+
```

### Comparing `transientNamer-0.4.5/setup.py` & `transientNamer-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `transientNamer-0.4.5/transientNamer/astronotes.py` & `transientNamer-0.4.6/transientNamer/astronotes.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 :Author:
     David Young
 
 :Date Created:
     January 15, 2021
 """
+from bs4 import BeautifulSoup
+import codecs
+import time
+from fundamentals.mysql import readquery
+from fundamentals.mysql import convert_dictionary_to_mysql_table
+from fundamentals.mysql import insert_list_of_dictionaries_into_database_tables
+from pprint import pprint
+import json
+import requests
+from fundamentals import tools
 from builtins import object
 import sys
 import re
 import os
 os.environ['TERM'] = 'vt100'
-from fundamentals import tools
-import requests
-import json
-from pprint import pprint
-from fundamentals.mysql import insert_list_of_dictionaries_into_database_tables
-from fundamentals.mysql import convert_dictionary_to_mysql_table
-from fundamentals.mysql import readquery
-import time
-import codecs
-from bs4 import BeautifulSoup
 
 
 class astronotes(object):
     """
     *Tools to download, parse and ingest astronote content into a MySQL database*
 
     **Key Arguments:**
@@ -548,15 +548,15 @@
                     dictList=results,
                     dbTableName="astronotes_transients",
                     uniqueKeyList=["astronote", "iauname"],
                     dateModified=True,
                     dateCreated=True,
                     batchSize=2500,
                     replace=True,
-                    # dbSettings=self.settings["database settings"]
+                    dbSettings=self.settings["database settings"]
                 )
 
         self.log.debug('completed the ``_parse_html_to_database`` method')
         return None
 
     # use the tab-trigger below for new method
     # xt-class-method
```

### Comparing `transientNamer-0.4.5/transientNamer/cl_utils.py` & `transientNamer-0.4.6/transientNamer/cl_utils.py`

 * *Files identical despite different names*

### Comparing `transientNamer-0.4.5/transientNamer/default_settings.yaml` & `transientNamer-0.4.6/transientNamer/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `transientNamer-0.4.5/transientNamer/search.py` & `transientNamer-0.4.6/transientNamer/search.py`

 * *Files identical despite different names*

### Comparing `transientNamer-0.4.5/transientNamer/test_settings.yaml` & `transientNamer-0.4.6/transientNamer/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `transientNamer-0.4.5/transientNamer/utKit.py` & `transientNamer-0.4.6/transientNamer/utKit.py`

 * *Files identical despite different names*

### Comparing `transientNamer-0.4.5/transientNamer.egg-info/PKG-INFO` & `transientNamer-0.4.6/transientNamer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: transientNamer
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python API for reading and caching TNS reports
 Home-page: https://github.com/thespacedoctor/transientNamer
-Download-URL: https://github.com/thespacedoctor/transientNamer/archive/v0.4.5.zip
+Download-URL: https://github.com/thespacedoctor/transientNamer/archive/v0.4.6.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: MIT
 Keywords: astronomy, transients
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # transientNamer
 
+
+
+[![](https://zenodo.org/badge/53676687.svg)](https://zenodo.org/badge/latestdoi/53676687) 
+
+
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/transientNamer)](https://pypi.org/project/transientNamer/)  
 [![](https://img.shields.io/pypi/v/transientNamer)](https://pypi.org/project/transientNamer/)  
 [![](https://img.shields.io/github/license/thespacedoctor/transientNamer)](https://github.com/thespacedoctor/transientNamer)  
 [![](https://img.shields.io/pypi/dm/transientNamer)](https://pypi.org/project/transientNamer/)  
 
@@ -36,9 +41,23 @@
 
 Documentation for transientNamer is hosted by [Read the Docs](https://transientNamer.readthedocs.io/en/master/) ([development version](https://transientNamer.readthedocs.io/en/develop/) and [master version](https://transientNamer.readthedocs.io/en/master/)). The code lives on [github](https://github.com/thespacedoctor/transientNamer). Please report any issues you find [here](https://github.com/thespacedoctor/transientNamer/issues).
 
 ## Features
 
 * 
 
+## How to cite transientNamer
+
+If you use `transientNamer` in your work, please cite using the following BibTeX entry: 
+
+```bibtex
+@software{Young_transientNamer,
+    author = {Young, David R.},
+    doi = {10.5281/zenodo.7970680},
+    license = {GPL-3.0-only},
+    title = {{transientNamer}},
+    url = {https://github.com/thespacedoctor/transientNamer}
+}
+```
+
```

### Comparing `transientNamer-0.4.5/transientNamer.egg-info/SOURCES.txt` & `transientNamer-0.4.6/transientNamer.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 transientNamer.egg-info/SOURCES.txt
 transientNamer.egg-info/dependency_links.txt
 transientNamer.egg-info/entry_points.txt
 transientNamer.egg-info/not-zip-safe
 transientNamer.egg-info/requires.txt
 transientNamer.egg-info/top_level.txt
 transientNamer/commonutils/__init__.py
-transientNamer/commonutils/getpackagepath.py
+transientNamer/commonutils/getpackagepath.py
+transientNamer/resources/package.mplstyle
```


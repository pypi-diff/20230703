# Comparing `tmp/helperfns-0.0.3.tar.gz` & `tmp/helperfns-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\helperfns-0.0.3.tar", last modified: Tue Sep  6 07:20:04 2022, max compression
+gzip compressed data, was "dist\helperfns-0.0.4.tar", last modified: Mon Jul  3 10:22:18 2023, max compression
```

## Comparing `helperfns-0.0.3.tar` & `helperfns-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-09-06 07:20:04.294451 helperfns-0.0.3/
--rw-rw-rw-   0        0        0     1089 2022-07-19 04:53:06.000000 helperfns-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     8223 2022-09-06 07:20:04.291449 helperfns-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6526 2022-09-01 10:27:40.000000 helperfns-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-09-06 07:20:04.209450 helperfns-0.0.3/helperfns/
--rw-rw-rw-   0        0        0        0 2022-07-19 06:30:21.000000 helperfns-0.0.3/helperfns/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 07:20:04.260447 helperfns-0.0.3/helperfns/tables/
--rw-rw-rw-   0        0        0     1944 2022-07-19 10:05:44.000000 helperfns-0.0.3/helperfns/tables/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 07:20:04.265450 helperfns-0.0.3/helperfns/text/
--rw-rw-rw-   0        0        0     4766 2022-09-01 09:10:36.000000 helperfns-0.0.3/helperfns/text/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 07:20:04.268450 helperfns-0.0.3/helperfns/torch/
--rw-rw-rw-   0        0        0        0 2022-09-01 09:23:02.000000 helperfns-0.0.3/helperfns/torch/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 07:20:04.272453 helperfns-0.0.3/helperfns/torch/accuracy/
--rw-rw-rw-   0        0        0     1981 2022-08-25 07:48:07.000000 helperfns-0.0.3/helperfns/torch/accuracy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 07:20:04.275449 helperfns-0.0.3/helperfns/torch/models/
--rw-rw-rw-   0        0        0      971 2022-09-06 05:59:54.000000 helperfns-0.0.3/helperfns/torch/models/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 07:20:04.279452 helperfns-0.0.3/helperfns/torch/text/
--rw-rw-rw-   0        0        0     4848 2022-09-01 10:27:12.000000 helperfns-0.0.3/helperfns/torch/text/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 07:20:04.283455 helperfns-0.0.3/helperfns/utils/
--rw-rw-rw-   0        0        0      775 2022-08-25 07:27:13.000000 helperfns-0.0.3/helperfns/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 07:20:04.286451 helperfns-0.0.3/helperfns/visualization/
--rw-rw-rw-   0        0        0     8989 2022-07-19 07:52:44.000000 helperfns-0.0.3/helperfns/visualization/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 07:20:04.253447 helperfns-0.0.3/helperfns.egg-info/
--rw-rw-rw-   0        0        0     8223 2022-09-06 07:20:02.000000 helperfns-0.0.3/helperfns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2022-09-06 07:20:04.000000 helperfns-0.0.3/helperfns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-06 07:20:02.000000 helperfns-0.0.3/helperfns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-09-06 07:20:03.000000 helperfns-0.0.3/helperfns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-09-06 07:20:03.000000 helperfns-0.0.3/helperfns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-06 07:20:04.295449 helperfns-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1987 2022-09-06 07:19:47.000000 helperfns-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.464961 helperfns-0.0.4/
+-rw-rw-rw-   0        0        0     1089 2022-07-19 04:53:06.000000 helperfns-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     8223 2023-07-03 10:22:18.454963 helperfns-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6526 2022-09-01 10:27:40.000000 helperfns-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.345964 helperfns-0.0.4/helperfns/
+-rw-rw-rw-   0        0        0        0 2022-07-19 06:30:21.000000 helperfns-0.0.4/helperfns/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.417960 helperfns-0.0.4/helperfns/tables/
+-rw-rw-rw-   0        0        0     1917 2023-07-03 10:15:06.000000 helperfns-0.0.4/helperfns/tables/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.423964 helperfns-0.0.4/helperfns/text/
+-rw-rw-rw-   0        0        0     4766 2022-09-01 09:10:36.000000 helperfns-0.0.4/helperfns/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.427959 helperfns-0.0.4/helperfns/torch/
+-rw-rw-rw-   0        0        0        0 2022-09-01 09:23:02.000000 helperfns-0.0.4/helperfns/torch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.430962 helperfns-0.0.4/helperfns/torch/accuracy/
+-rw-rw-rw-   0        0        0     1981 2022-08-25 07:48:07.000000 helperfns-0.0.4/helperfns/torch/accuracy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.434971 helperfns-0.0.4/helperfns/torch/models/
+-rw-rw-rw-   0        0        0      971 2022-09-06 05:59:54.000000 helperfns-0.0.4/helperfns/torch/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.440964 helperfns-0.0.4/helperfns/torch/text/
+-rw-rw-rw-   0        0        0     4848 2022-09-01 10:27:12.000000 helperfns-0.0.4/helperfns/torch/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.444962 helperfns-0.0.4/helperfns/utils/
+-rw-rw-rw-   0        0        0      775 2022-08-25 07:27:13.000000 helperfns-0.0.4/helperfns/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.448963 helperfns-0.0.4/helperfns/visualization/
+-rw-rw-rw-   0        0        0     8989 2022-07-19 07:52:44.000000 helperfns-0.0.4/helperfns/visualization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.413959 helperfns-0.0.4/helperfns.egg-info/
+-rw-rw-rw-   0        0        0     8223 2023-07-03 10:22:16.000000 helperfns-0.0.4/helperfns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-07-03 10:22:18.000000 helperfns-0.0.4/helperfns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 10:22:17.000000 helperfns-0.0.4/helperfns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-03 10:22:17.000000 helperfns-0.0.4/helperfns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 10:22:17.000000 helperfns-0.0.4/helperfns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 10:22:18.465962 helperfns-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1989 2023-07-03 10:10:38.000000 helperfns-0.0.4/setup.py
```

### Comparing `helperfns-0.0.3/LICENSE` & `helperfns-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.3/PKG-INFO` & `helperfns-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helperfns
-Version: 0.0.3
+Version: 0.0.4
 Summary: This package provide some python helper functions that are useful in machine learning.
 Author: Crispen Gari
 Author-email: <crispengari@gmail.com>
 Keywords: python,python3,helper-functions,text cleaning,visualization,machine-learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `helperfns-0.0.3/README.md` & `helperfns-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.3/helperfns/tables/__init__.py` & `helperfns-0.0.4/helperfns/tables/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from prettytable import PrettyTable
 
 
 def tabulate_data(column_names: list, data: list, title: str = "Table"):
-    
+
     """
     Tabulate Data
 
     This function print the data in a nice table format.
 
     Parameters
     ----------
     column_names : list
         These are table headers.
     labels_true : list
         Takes in a collection of correct labels.
     data : list
         The data that you want to print in table format.
-        
+
     Keyword Args
     ------------
     title : str
         The table title, the default title is "Table".
-        
+
     Returns
     -------
     None
 
     See Also
     --------
     tabulate_translations: Tabulate translation data with translation target paired to translation source.
@@ -44,18 +44,19 @@
     | validation |          4 |     4 |
     | test       |          3 |       |
     +------------+------------+-------+
     """
     assert len(data) != 0, f"Data is required but got nothing."
     assert len(column_names) == len(data[0]), f"Column names and data must have the same length, but got {len(column_names)} and {len(data)}."
     assert all([len(d)== len(data[0]) for d in data]), f"The row data must have the same length."
-    
+
     table = PrettyTable(column_names)
-    table.title = title
     for i, name in enumerate(column_names):
         if(i == 0):
             table.align[name] = 'l'
         else:
             table.align[name] = 'r'
     for row in data:
         table.add_row(row)
-    print(table)
+
+    print(title)
+    print(table)
```

### Comparing `helperfns-0.0.3/helperfns/text/__init__.py` & `helperfns-0.0.4/helperfns/text/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.3/helperfns/torch/accuracy/__init__.py` & `helperfns-0.0.4/helperfns/torch/accuracy/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.3/helperfns/torch/models/__init__.py` & `helperfns-0.0.4/helperfns/torch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.3/helperfns/torch/text/__init__.py` & `helperfns-0.0.4/helperfns/torch/text/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.3/helperfns/utils/__init__.py` & `helperfns-0.0.4/helperfns/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.3/helperfns/visualization/__init__.py` & `helperfns-0.0.4/helperfns/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.3/helperfns.egg-info/PKG-INFO` & `helperfns-0.0.4/helperfns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helperfns
-Version: 0.0.3
+Version: 0.0.4
 Summary: This package provide some python helper functions that are useful in machine learning.
 Author: Crispen Gari
 Author-email: <crispengari@gmail.com>
 Keywords: python,python3,helper-functions,text cleaning,visualization,machine-learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `helperfns-0.0.3/setup.py` & `helperfns-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = "This package provide some python helper functions that are useful in machine learning."
 # setting up
 setup(
     name="helperfns",
     version=VERSION,
     author="Crispen Gari",
     author_email="<crispengari@gmail.com>",
@@ -46,8 +46,8 @@
         "Topic :: Utilities",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
-)
+)
```


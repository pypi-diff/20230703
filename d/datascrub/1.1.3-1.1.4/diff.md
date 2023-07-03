# Comparing `tmp/datascrub-1.1.3.tar.gz` & `tmp/datascrub-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascrub-1.1.3.tar", last modified: Mon Jul  3 10:17:20 2023, max compression
+gzip compressed data, was "datascrub-1.1.4.tar", last modified: Mon Jul  3 10:32:54 2023, max compression
```

## Comparing `datascrub-1.1.3.tar` & `datascrub-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-07-03 10:17:20.549403 datascrub-1.1.3/
--rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 datascrub-1.1.3/LICENSE.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)     2653 2023-07-03 10:17:20.549265 datascrub-1.1.3/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)     1977 2023-06-22 11:41:41.000000 datascrub-1.1.3/README.md
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-07-03 10:17:20.548180 datascrub-1.1.3/datascrub/
--rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 06:32:25.000000 datascrub-1.1.3/datascrub/__init__.py
--rw-r--r--   0 samuelshine   (501) staff       (20)     9499 2023-07-03 10:14:23.000000 datascrub-1.1.3/datascrub/cleaner.py
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-07-03 10:17:20.548965 datascrub-1.1.3/datascrub.egg-info/
--rw-r--r--   0 samuelshine   (501) staff       (20)     2653 2023-07-03 10:17:20.000000 datascrub-1.1.3/datascrub.egg-info/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)      237 2023-07-03 10:17:20.000000 datascrub-1.1.3/datascrub.egg-info/SOURCES.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-07-03 10:17:20.000000 datascrub-1.1.3/datascrub.egg-info/dependency_links.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-07-03 10:17:20.000000 datascrub-1.1.3/datascrub.egg-info/requires.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       10 2023-07-03 10:17:20.000000 datascrub-1.1.3/datascrub.egg-info/top_level.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-07-03 10:17:20.549445 datascrub-1.1.3/setup.cfg
--rw-r--r--   0 samuelshine   (501) staff       (20)     1014 2023-07-03 10:16:49.000000 datascrub-1.1.3/setup.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-07-03 10:32:54.217169 datascrub-1.1.4/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 datascrub-1.1.4/LICENSE.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)     2907 2023-07-03 10:32:54.217045 datascrub-1.1.4/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)     2231 2023-07-03 10:32:14.000000 datascrub-1.1.4/README.md
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-07-03 10:32:54.216010 datascrub-1.1.4/datascrub/
+-rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 06:32:25.000000 datascrub-1.1.4/datascrub/__init__.py
+-rw-r--r--   0 samuelshine   (501) staff       (20)     9499 2023-07-03 10:14:23.000000 datascrub-1.1.4/datascrub/cleaner.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-07-03 10:32:54.216850 datascrub-1.1.4/datascrub.egg-info/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     2907 2023-07-03 10:32:54.000000 datascrub-1.1.4/datascrub.egg-info/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)      237 2023-07-03 10:32:54.000000 datascrub-1.1.4/datascrub.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-07-03 10:32:54.000000 datascrub-1.1.4/datascrub.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-07-03 10:32:54.000000 datascrub-1.1.4/datascrub.egg-info/requires.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       10 2023-07-03 10:32:54.000000 datascrub-1.1.4/datascrub.egg-info/top_level.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-07-03 10:32:54.217214 datascrub-1.1.4/setup.cfg
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1014 2023-07-03 10:32:31.000000 datascrub-1.1.4/setup.py
```

### Comparing `datascrub-1.1.3/LICENSE.txt` & `datascrub-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datascrub-1.1.3/PKG-INFO` & `datascrub-1.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: datascrub
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python package for cleaning and preprocessing data in pandas DataFrames
 Home-page: https://github.com/samuelshine/cleanmydata
 Author: Alex Benjamin
 Author-email: samuelshine112003@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Certainly! Here's an updated README file for your DataScrub package:
-
----
-
 # DataScrub
 
 DataScrub is a Python package that provides powerful data cleaning and preprocessing capabilities for pandas DataFrames. It offers a collection of functions and utilities to facilitate data cleaning tasks, handling missing values, standardizing data formats, and more. With DataScrub, you can streamline your data preparation process and ensure the quality and consistency of your datasets.
 
+## Features
+
+- Clean text data in pandas DataFrames
+- Handle missing values with customizable actions
+- Perform scaling normalization on numerical columns
+- Split and expand data in specified columns
+- Convert columns to datetime format and format them as 'YYYY-MM-DD'
+- Translate text columns to English using Google Translate
+
 ## Installation
 
 DataScrub can be easily installed using pip. Simply run the following command:
 
 ```shell
 pip install datascrub
 ```
@@ -45,15 +50,15 @@
 data = pd.read_csv("data.csv")
 
 # Create an instance of DataClean
 cleaner = DataClean(data)
 
 # Call the available methods to clean and preprocess your data
 cleaned_data = cleaner.prep(clean='all', missing_values={}, perform_scaling_normalization_bool=False,
-                            explode={}, parse_date=[], translate_column_names={})
+                            explode={}, parse_date={}, translate_column_names={})
 ```
 
 The `DataClean` class takes a pandas DataFrame or a file path as input. You can then use the various methods available in the class to clean and preprocess your data.
 
 Refer to the [documentation](https://github.com/samuelshine/datascrub) for detailed information on available methods and usage examples.
 
 ## Contributing
```

### Comparing `datascrub-1.1.3/README.md` & `datascrub-1.1.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-Certainly! Here's an updated README file for your DataScrub package:
-
----
-
 # DataScrub
 
 DataScrub is a Python package that provides powerful data cleaning and preprocessing capabilities for pandas DataFrames. It offers a collection of functions and utilities to facilitate data cleaning tasks, handling missing values, standardizing data formats, and more. With DataScrub, you can streamline your data preparation process and ensure the quality and consistency of your datasets.
 
+## Features
+
+- Clean text data in pandas DataFrames
+- Handle missing values with customizable actions
+- Perform scaling normalization on numerical columns
+- Split and expand data in specified columns
+- Convert columns to datetime format and format them as 'YYYY-MM-DD'
+- Translate text columns to English using Google Translate
+
 ## Installation
 
 DataScrub can be easily installed using pip. Simply run the following command:
 
 ```shell
 pip install datascrub
 ```
@@ -28,15 +33,15 @@
 data = pd.read_csv("data.csv")
 
 # Create an instance of DataClean
 cleaner = DataClean(data)
 
 # Call the available methods to clean and preprocess your data
 cleaned_data = cleaner.prep(clean='all', missing_values={}, perform_scaling_normalization_bool=False,
-                            explode={}, parse_date=[], translate_column_names={})
+                            explode={}, parse_date={}, translate_column_names={})
 ```
 
 The `DataClean` class takes a pandas DataFrame or a file path as input. You can then use the various methods available in the class to clean and preprocess your data.
 
 Refer to the [documentation](https://github.com/samuelshine/datascrub) for detailed information on available methods and usage examples.
 
 ## Contributing
```

### Comparing `datascrub-1.1.3/datascrub/cleaner.py` & `datascrub-1.1.4/datascrub/cleaner.py`

 * *Files identical despite different names*

### Comparing `datascrub-1.1.3/datascrub.egg-info/PKG-INFO` & `datascrub-1.1.4/datascrub.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: datascrub
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python package for cleaning and preprocessing data in pandas DataFrames
 Home-page: https://github.com/samuelshine/cleanmydata
 Author: Alex Benjamin
 Author-email: samuelshine112003@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Certainly! Here's an updated README file for your DataScrub package:
-
----
-
 # DataScrub
 
 DataScrub is a Python package that provides powerful data cleaning and preprocessing capabilities for pandas DataFrames. It offers a collection of functions and utilities to facilitate data cleaning tasks, handling missing values, standardizing data formats, and more. With DataScrub, you can streamline your data preparation process and ensure the quality and consistency of your datasets.
 
+## Features
+
+- Clean text data in pandas DataFrames
+- Handle missing values with customizable actions
+- Perform scaling normalization on numerical columns
+- Split and expand data in specified columns
+- Convert columns to datetime format and format them as 'YYYY-MM-DD'
+- Translate text columns to English using Google Translate
+
 ## Installation
 
 DataScrub can be easily installed using pip. Simply run the following command:
 
 ```shell
 pip install datascrub
 ```
@@ -45,15 +50,15 @@
 data = pd.read_csv("data.csv")
 
 # Create an instance of DataClean
 cleaner = DataClean(data)
 
 # Call the available methods to clean and preprocess your data
 cleaned_data = cleaner.prep(clean='all', missing_values={}, perform_scaling_normalization_bool=False,
-                            explode={}, parse_date=[], translate_column_names={})
+                            explode={}, parse_date={}, translate_column_names={})
 ```
 
 The `DataClean` class takes a pandas DataFrame or a file path as input. You can then use the various methods available in the class to clean and preprocess your data.
 
 Refer to the [documentation](https://github.com/samuelshine/datascrub) for detailed information on available methods and usage examples.
 
 ## Contributing
```

### Comparing `datascrub-1.1.3/setup.py` & `datascrub-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='datascrub',
-    version='1.1.3',
+    version='1.1.4',
     author='Samuel Shine' and 'Alex Benjamin',
     author_email='samuelshine112003@gmail.com',
     description='A Python package for cleaning and preprocessing data in pandas DataFrames',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/samuelshine/cleanmydata',
     packages=find_packages(),
```


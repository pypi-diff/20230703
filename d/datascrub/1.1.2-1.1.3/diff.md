# Comparing `tmp/datascrub-1.1.2.tar.gz` & `tmp/datascrub-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascrub-1.1.2.tar", last modified: Thu Jun 22 11:28:23 2023, max compression
+gzip compressed data, was "datascrub-1.1.3.tar", last modified: Mon Jul  3 10:17:20 2023, max compression
```

## Comparing `datascrub-1.1.2.tar` & `datascrub-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 11:28:23.651081 datascrub-1.1.2/
--rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 datascrub-1.1.2/LICENSE.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)     5610 2023-06-22 11:28:23.650956 datascrub-1.1.2/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)     4913 2023-06-22 06:10:32.000000 datascrub-1.1.2/README.md
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 11:28:23.650053 datascrub-1.1.2/datascrub/
--rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 06:32:25.000000 datascrub-1.1.2/datascrub/__init__.py
--rw-r--r--   0 samuelshine   (501) staff       (20)     9448 2023-06-22 11:27:58.000000 datascrub-1.1.2/datascrub/cleaner.py
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 11:28:23.650763 datascrub-1.1.2/datascrub.egg-info/
--rw-r--r--   0 samuelshine   (501) staff       (20)     5610 2023-06-22 11:28:23.000000 datascrub-1.1.2/datascrub.egg-info/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)      237 2023-06-22 11:28:23.000000 datascrub-1.1.2/datascrub.egg-info/SOURCES.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-06-22 11:28:23.000000 datascrub-1.1.2/datascrub.egg-info/dependency_links.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 11:28:23.000000 datascrub-1.1.2/datascrub.egg-info/requires.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       10 2023-06-22 11:28:23.000000 datascrub-1.1.2/datascrub.egg-info/top_level.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-06-22 11:28:23.651121 datascrub-1.1.2/setup.cfg
--rw-r--r--   0 samuelshine   (501) staff       (20)     1013 2023-06-22 11:28:18.000000 datascrub-1.1.2/setup.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-07-03 10:17:20.549403 datascrub-1.1.3/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 datascrub-1.1.3/LICENSE.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)     2653 2023-07-03 10:17:20.549265 datascrub-1.1.3/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1977 2023-06-22 11:41:41.000000 datascrub-1.1.3/README.md
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-07-03 10:17:20.548180 datascrub-1.1.3/datascrub/
+-rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 06:32:25.000000 datascrub-1.1.3/datascrub/__init__.py
+-rw-r--r--   0 samuelshine   (501) staff       (20)     9499 2023-07-03 10:14:23.000000 datascrub-1.1.3/datascrub/cleaner.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-07-03 10:17:20.548965 datascrub-1.1.3/datascrub.egg-info/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     2653 2023-07-03 10:17:20.000000 datascrub-1.1.3/datascrub.egg-info/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)      237 2023-07-03 10:17:20.000000 datascrub-1.1.3/datascrub.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-07-03 10:17:20.000000 datascrub-1.1.3/datascrub.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-07-03 10:17:20.000000 datascrub-1.1.3/datascrub.egg-info/requires.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       10 2023-07-03 10:17:20.000000 datascrub-1.1.3/datascrub.egg-info/top_level.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-07-03 10:17:20.549445 datascrub-1.1.3/setup.cfg
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1014 2023-07-03 10:16:49.000000 datascrub-1.1.3/setup.py
```

### Comparing `datascrub-1.1.2/LICENSE.txt` & `datascrub-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datascrub-1.1.2/datascrub/cleaner.py` & `datascrub-1.1.3/datascrub/cleaner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import pandas as pd
 import numpy as np
 import datetime
 import charset_normalizer
-import fuzzywuzzy
-from fuzzywuzzy import process
 import re
 from scipy import stats
 from pandas.api.types import is_numeric_dtype
 import emoji
 import string
 from googletrans import Translator
 
@@ -131,28 +129,28 @@
         return self.raw_data.drop_duplicates()
 
     def parse_date_column(self, date_columns):
         """
         Converts specified columns in a pandas DataFrame to datetime format and formats them as 'YYYY-MM-DD'.
 
         Parameters:
-        date_columns (dict): List of column names to be converted to datetime format.
+        date_columns (dict): Dictionary of column names to be converted to datetime format.
 
         Returns:
         pd.DataFrame: DataFrame with parsed date columns.
         """
         updated_data = self.raw_data.copy()
 
-        for column in date_columns:
+        for column, dformat in date_columns.items():
             if column not in updated_data.columns:
                 raise ValueError(f"Column '{column}' not found in the DataFrame.")
 
             if updated_data[column].dtype != 'datetime64[ns]':
                 updated_data[column] = updated_data[column].astype(str)
-                updated_data[column] = pd.to_datetime(updated_data[column], errors='coerce').dt.strftime('%Y-%m-%d')
+                updated_data[column] = pd.to_datetime(updated_data[column], format=dformat, errors='coerce').dt.strftime('%Y-%m-%d')
                 # updated_data[column] = pd.to_datetime(updated_data[column], format=date_format)
 
         return updated_data
 
     def translate_columns(self, translations):
         """
         Translates text in specified columns of a DataFrame to English using Google Translate.
@@ -181,25 +179,25 @@
                 updated_data[column] = translated_texts
             else:
                 new_column_name = column + '_translated'
                 updated_data[new_column_name] = translated_texts
 
         return updated_data
 
-    def prep(self, clean='all', missing_values={}, perform_scaling_normalization_bool=False, explode={}, parse_date=[], translate_column_names={}):
+    def prep(self, clean='all', missing_values={}, perform_scaling_normalization_bool=False, explode={}, parse_date={}, translate_column_names={}):
         """
         Main function to prepare and clean a pandas DataFrame. Can perform cleaning, handle missing values, fix inconsistencies,
         perform scaling normalization, explode data, and parse date columns based on parameters passed.
 
         Parameters:
         clean (str, list): Columns to clean. Either 'all' for all columns or a list of specific column names.
         missing_values (dict): Actions to be taken on missing values. Refer `handle_missing_values` for more details.
         perform_scaling_normalization (bool): If True, will perform scaling normalization on numerical columns.
         explode (dict): Columns to be exploded. Keys are column names and values are separators for splitting.
-        parse_date (list): List of column names to be converted to datetime format.
+        parse_date (dict): Dictionary of column names to be converted to datetime format, with format as the values and column names as the key.
         translate_column_names (dict): Dictionary mapping column names to overwrite boolean values for translation.
 
         Returns:
         pd.DataFrame: Updated DataFrame with cleaned and processed data.
         """
         if missing_values:
             self.raw_data = self.handle_missing_values(missing_values)
```

### Comparing `datascrub-1.1.2/setup.py` & `datascrub-1.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='datascrub',
-    version='1.1.2',
-    author=['Samuel Shine', 'Alex Benjamin'],
+    version='1.1.3',
+    author='Samuel Shine' and 'Alex Benjamin',
     author_email='samuelshine112003@gmail.com',
     description='A Python package for cleaning and preprocessing data in pandas DataFrames',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/samuelshine/cleanmydata',
     packages=find_packages(),
     classifiers=[
```


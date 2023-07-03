# Comparing `tmp/veetility-0.1.93.tar.gz` & `tmp/veetility-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veetility-0.1.93.tar", last modified: Fri Jun 30 16:47:07 2023, max compression
+gzip compressed data, was "veetility-0.1.94.tar", last modified: Mon Jul  3 13:10:51 2023, max compression
```

## Comparing `veetility-0.1.93.tar` & `veetility-0.1.94.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-30 16:47:07.903759 veetility-0.1.93/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-30 16:47:07.903602 veetility-0.1.93/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.93/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-06-30 16:47:07.903812 veetility-0.1.93/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-06-30 16:46:59.000000 veetility-0.1.93/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-30 16:47:07.898795 veetility-0.1.93/tests/
--rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.93/tests/test_best_fuzzy_match_dict.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.93/tests/test_identify_match_multi_cols.py
--rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.93/tests/test_prepare_string_matching.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-30 16:47:07.902376 veetility-0.1.93/veetility/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.93/veetility/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    17689 2023-06-27 09:01:02.000000 veetility-0.1.93/veetility/cleaning_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.93/veetility/generic_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.93/veetility/point_to_point_regressor.py
--rw-r--r--   0 willbutler   (502) staff       (20)    31084 2023-06-30 16:44:04.000000 veetility-0.1.93/veetility/quality_assessments.py
--rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.93/veetility/snowflake.py
--rw-r--r--   0 willbutler   (502) staff       (20)    53597 2023-06-26 09:44:14.000000 veetility-0.1.93/veetility/utility_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.93/veetility/v_lift.py
--rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.93/veetility/view_through_rate.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-30 16:47:07.903382 veetility-0.1.93/veetility.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-30 16:47:07.000000 veetility-0.1.93/veetility.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-06-30 16:47:07.000000 veetility-0.1.93/veetility.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-06-30 16:47:07.000000 veetility-0.1.93/veetility.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-06-30 16:47:07.000000 veetility-0.1.93/veetility.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-06-30 16:47:07.000000 veetility-0.1.93/veetility.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-03 13:10:51.598542 veetility-0.1.94/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-03 13:10:51.598381 veetility-0.1.94/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.94/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-07-03 13:10:51.598599 veetility-0.1.94/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-07-03 13:10:47.000000 veetility-0.1.94/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-03 13:10:51.593708 veetility-0.1.94/tests/
+-rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.94/tests/test_best_fuzzy_match_dict.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.94/tests/test_identify_match_multi_cols.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.94/tests/test_prepare_string_matching.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-03 13:10:51.596959 veetility-0.1.94/veetility/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.94/veetility/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    17689 2023-06-27 09:01:02.000000 veetility-0.1.94/veetility/cleaning_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.94/veetility/generic_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.94/veetility/point_to_point_regressor.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    31242 2023-07-03 13:10:09.000000 veetility-0.1.94/veetility/quality_assessments.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.94/veetility/snowflake.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    53597 2023-06-26 09:44:14.000000 veetility-0.1.94/veetility/utility_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.94/veetility/v_lift.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.94/veetility/view_through_rate.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-03 13:10:51.598015 veetility-0.1.94/veetility.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-03 13:10:51.000000 veetility-0.1.94/veetility.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-07-03 13:10:51.000000 veetility-0.1.94/veetility.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-07-03 13:10:51.000000 veetility-0.1.94/veetility.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-07-03 13:10:51.000000 veetility-0.1.94/veetility.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-07-03 13:10:51.000000 veetility-0.1.94/veetility.egg-info/top_level.txt
```

### Comparing `veetility-0.1.93/PKG-INFO` & `veetility-0.1.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.93
+Version: 0.1.94
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.93/README.md` & `veetility-0.1.94/README.md`

 * *Files identical despite different names*

### Comparing `veetility-0.1.93/setup.py` & `veetility-0.1.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="veetility",
-    version="0.1.93",
+    version="0.1.94",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Vaynermedia",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `veetility-0.1.93/tests/test_best_fuzzy_match_dict.py` & `veetility-0.1.94/tests/test_best_fuzzy_match_dict.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.93/tests/test_identify_match_multi_cols.py` & `veetility-0.1.94/tests/test_identify_match_multi_cols.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.93/tests/test_prepare_string_matching.py` & `veetility-0.1.94/tests/test_prepare_string_matching.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.93/veetility/cleaning_functions.py` & `veetility-0.1.94/veetility/cleaning_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.93/veetility/generic_functions.py` & `veetility-0.1.94/veetility/generic_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.93/veetility/point_to_point_regressor.py` & `veetility-0.1.94/veetility/point_to_point_regressor.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.93/veetility/quality_assessments.py` & `veetility-0.1.94/veetility/quality_assessments.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,97 +167,96 @@
         # return TT or IG values with empty message field
         # for the date function exlude the dates we paused for the queen
 
         logger.warning(error_message)
         return error_message
     
     def comparison_with_previous_data(self, df, name_of_df, cols_to_check=['impressions','likes'], perc_increase_threshold=20,
-                                   perc_decrease_threshold=0.5, check_cols_set=True, raise_exceptions=False):
-        """ This function stores the high level sums for a datatable from the previous run of the script
-        and if they have reduced or increased too sharply an error is raised.
-
-        A JSON file is created which stores historical data about the dataframe, the columns present and the
-        sum of the columns specified in cols_to_check. This can then be used for reference purposes to see if any changes in the totals are
-        caused by code changes or errors. 
-
-        Args:
-            df (pd.DataFrame): Input dataframe that the historic checks are going to be performed on.
-            name_of_df (str): Name of the dataframe, this will be used to name a file to save for future comparison.
-            cols_to_check (List[str]): A list of strings that detail the columns to be totaled which will then 
-                be compared with previous data.
-            perc_increase_threshold (float): A number between 0 and 100, the percentage increase threshold above 
-                which it is deemed that the totals have raised too rapidly and an error has occured.
-            perc_decrease_threshold (float): A number between 0 and 100, the percentage decrease threshold below 
-                which it is deemed that the totals decreased and an error has occured.
-            check_cols_set (bool): If true, store the set of columns present for comparison to see if any new 
-                columns have been added or removed next time, in which case it is deemed an error has occured.
-            raise_exceptions (bool): If true, then raise an exception if an error has occured instead of just returning an error message.
-
-        Returns:
-            error_message (str): String detailing what the error is so that it can be passed to a notification service like slack."""
-        
-        error_message, error_occured = '', False
-
-        # Create a dictionary of the sums of the columns specified in cols_to_check
-        new_dict = {}
-        new_dict['Date'] = str(datetime.now())
-        for col in cols_to_check:
-            new_dict[col] = int(df[col].sum())
-        if check_cols_set == True:
-            new_dict['Columns'] = df.columns.tolist()
-        
-        # Check if the historic database already exists, if not create it
-        client_name = self.util.client_name.lower()
-        if self.util.table_exists(f'{client_name}_{name_of_df}_previous_totals'):
-            historic_db = self.util.read_from_postgresql(f'{client_name}_{name_of_df}_previous_totals', clean_date=False)
-            historic_db.drop(columns=['DateWrittenToDB'], inplace=True) # This column is not needed for comparison, it gets created when writing to the db
-            historic_db = historic_db.reset_index()
-        else:
-            columns = ['Date'].extend(cols_to_check)
+                                    perc_decrease_threshold=0.5, check_cols_set=True, raise_exceptions=False):
+            """ This function stores the high level sums for a datatable from the previous run of the script
+            and if they have reduced or increased too sharply an error is raised.
+
+            A JSON file is created which stores historical data about the dataframe, the columns present and the
+            sum of the columns specified in cols_to_check. This can then be used for reference purposes to see if any changes in the totals are
+            caused by code changes or errors. 
+
+            Args:
+                df (pd.DataFrame): Input dataframe that the historic checks are going to be performed on.
+                name_of_df (str): Name of the dataframe, this will be used to name a file to save for future comparison.
+                cols_to_check (List[str]): A list of strings that detail the columns to be totaled which will then 
+                    be compared with previous data.
+                perc_increase_threshold (float): A number between 0 and 100, the percentage increase threshold above 
+                    which it is deemed that the totals have raised too rapidly and an error has occured.
+                perc_decrease_threshold (float): A number between 0 and 100, the percentage decrease threshold below 
+                    which it is deemed that the totals decreased and an error has occured.
+                check_cols_set (bool): If true, store the set of columns present for comparison to see if any new 
+                    columns have been added or removed next time, in which case it is deemed an error has occured.
+                raise_exceptions (bool): If true, then raise an exception if an error has occured instead of just returning an error message.
+
+            Returns:
+                error_message (str): String detailing what the error is so that it can be passed to a notification service like slack."""
+            
+            error_message, error_occured = '', False
+
+            # Create a dictionary of the sums of the columns specified in cols_to_check
+            new_dict = {}
+            new_dict['Date'] = str(datetime.now())
+            for col in cols_to_check:
+                new_dict[col] = int(df[col].sum())
             if check_cols_set == True:
-                columns.append('Columns')
-            historic_db = pd.DataFrame(columns=columns)
-            self.util.write_to_postgresql(historic_db, f'{client_name}_{name_of_df}_previous_totals', if_exists='replace')
-            return error_message
-        
-        #Turn the most recent entry in the historic db into a dict
-        old_dict = historic_db.sort_values(by='Date', ascending=False).iloc[0].to_dict()
-
-        # for each key in the old dict, check if it is in the new dict and if it is, check if it has increased or decreased too much
-        for key, value in old_dict.items():
-            if key == 'Columns':
-                if set(value) != set(new_dict['Columns']):
+                new_dict['Columns'] = df.columns.tolist()
+            
+            # Check if the historic database already exists, if not create it
+            client_name = self.util.client_name.lower()
+            if self.util.table_exists(f'{client_name}_{name_of_df}_previous_totals'):
+                historic_db = self.util.read_from_postgresql(f'{client_name}_{name_of_df}_previous_totals', clean_date=False)
+                historic_db.drop(columns=['DateWrittenToDB'], inplace=True) # This column is not needed for comparison, it gets created when writing to the db
+                historic_db = historic_db.reset_index(drop=True)
+
+            else:
+                historic_db = pd.DataFrame([new_dict])
+                self.util.write_to_postgresql(historic_db, f'{client_name}_{name_of_df}_previous_totals', if_exists='replace')
+                return error_message
+            
+            #Turn the most recent entry in the historic db into a dict
+            old_dict = historic_db.sort_values(by='Date', ascending=False).iloc[0].to_dict()
+
+            # for each key in the old dict, check if it is in the new dict and if it is, check if it has increased or decreased too much
+            for key, value in old_dict.items():
+
+                if key == 'Columns':
+                    if set(value) != set(new_dict['Columns']):
+                        error_occured = True
+                        columns_removed = list(set(value) - set(new_dict['Columns']))
+                        columns_added = list(set(new_dict['Columns']) - set(value))
+                        error_message = error_message + '  ' + f'The columns seems to have changed from last time,\n'\
+                                                f' Columns that were added = {columns_added}\n' \
+                                                f' Columns that were removed = {columns_removed}\n'
+                elif key == 'Date':
+                    continue
+                elif new_dict[key] * (1 + perc_decrease_threshold/100) < value:
                     error_occured = True
-                    columns_removed = list(set(value) - set(new_dict['Columns']))
-                    columns_added = list(set(new_dict['Columns']) - set(value))
-                    error_message = error_message + '  ' + f'The columns seems to have changed from last time,\n'\
-                                            f' Columns that were added = {columns_added}\n' \
-                                            f' Columns that were removed = {columns_removed}\n'
-            elif key == 'datetime':
-                continue
-            elif new_dict[key] *(1+perc_decrease_threshold/100) < value:
-                error_occured = True
-                error_message = error_message + '  ' + f'The total of {key} seems to have decreased from last time\n'\
-                                        f' Prev Value = {old_dict[key]} , New Value = {new_dict[key]}\n'
-            elif new_dict[key] > value*(1 +perc_increase_threshold/100):
-                error_occured = True
-                error_message = error_message + '  ' + f'The total of {key} has increased by more than\n'\
-                                    f'{perc_increase_threshold}% from last time\n'\
-                                        f' Prev Value = {old_dict[key]}, New Value = {new_dict[key]}\n'
-
-        if error_occured:
-            error_message = f'Comparison with historic df {name_of_df}: ' + error_message +'\n'
-            logger.info('ERROR' + error_message) # If error messages has been added to then log it
-        if raise_exceptions and error_occured:
-            raise Exception(error_message)
-        
-        db_with_new_row = pd.concat([historic_db, pd.DataFrame(new_dict, index=[0])], ignore_index=True)
-        self.util.write_to_postgresql(db_with_new_row, f'{client_name}_{name_of_df}_previous_totals', if_exists='append')
-        
-        return error_message
+                    error_message = error_message + '  ' + f'The total of {key} seems to have decreased from last time\n'\
+                                            f' Prev Value = {old_dict[key]} , New Value = {new_dict[key]}\n'
+                elif new_dict[key] > value * (1 + perc_increase_threshold/100):
+                    error_occured = True
+                    error_message = error_message + '  ' + f'The total of {key} has increased by more than\n'\
+                                        f'{perc_increase_threshold}% from last time\n'\
+                                            f' Prev Value = {old_dict[key]}, New Value = {new_dict[key]}\n'
+
+            if error_occured:
+                error_message = f'Comparison with historic df {name_of_df}: ' + error_message +'\n'
+                logger.info('ERROR' + error_message) # If error messages has been added to then log it
+            if raise_exceptions and error_occured:
+                raise Exception(error_message)
+            
+            db_with_new_row = pd.concat([historic_db, pd.DataFrame([new_dict])], ignore_index=True)
+            self.util.write_to_postgresql(db_with_new_row, f'{client_name}_{name_of_df}_previous_totals', if_exists='append')
+            
+            return error_message
     
     def duplicates_qa(self, df: pd.DataFrame, df_name: str, subset= None, drop_duplicates: bool = True):
         """Checks for duplicates and optionally drops duplicates in a dataframe.
         
         Args:
             df (pd.DataFrame): The Dataframe to be checked for duplicates
             df_name (str): The name of the dataframe to be used for logging purposes
```

### Comparing `veetility-0.1.93/veetility/snowflake.py` & `veetility-0.1.94/veetility/snowflake.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.93/veetility/utility_functions.py` & `veetility-0.1.94/veetility/utility_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.93/veetility/v_lift.py` & `veetility-0.1.94/veetility/v_lift.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.93/veetility/view_through_rate.py` & `veetility-0.1.94/veetility/view_through_rate.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.93/veetility.egg-info/PKG-INFO` & `veetility-0.1.94/veetility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.93
+Version: 0.1.94
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.93/veetility.egg-info/SOURCES.txt` & `veetility-0.1.94/veetility.egg-info/SOURCES.txt`

 * *Files identical despite different names*


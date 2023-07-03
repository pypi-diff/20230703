# Comparing `tmp/excel2mssql-0.0.1.tar.gz` & `tmp/excel2mssql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel2mssql-0.0.1.tar", last modified: Mon Jul  3 19:03:02 2023, max compression
+gzip compressed data, was "excel2mssql-0.0.2.tar", last modified: Mon Jul  3 19:50:25 2023, max compression
```

## Comparing `excel2mssql-0.0.1.tar` & `excel2mssql-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 19:03:02.947940 excel2mssql-0.0.1/
--rw-rw-rw-   0        0        0     1099 2023-07-03 13:35:18.000000 excel2mssql-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3403 2023-07-03 19:03:02.942730 excel2mssql-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2909 2023-07-03 18:40:38.000000 excel2mssql-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 19:03:02.889907 excel2mssql-0.0.1/app/
--rw-rw-rw-   0        0        0        0 2023-07-03 13:42:05.000000 excel2mssql-0.0.1/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 19:03:02.894567 excel2mssql-0.0.1/app/data/
--rw-rw-rw-   0        0        0        0 2023-07-03 16:22:52.000000 excel2mssql-0.0.1/app/data/__init__.py
--rw-rw-rw-   0        0        0      141 2023-07-03 16:26:15.000000 excel2mssql-0.0.1/app/data/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-03 19:03:02.905075 excel2mssql-0.0.1/app/excel2mssql/
--rw-rw-rw-   0        0        0        0 2023-07-03 13:42:30.000000 excel2mssql-0.0.1/app/excel2mssql/__init__.py
--rw-rw-rw-   0        0        0     8002 2023-07-03 17:50:18.000000 excel2mssql-0.0.1/app/excel2mssql/excel2mssql.py
-drwxrwxrwx   0        0        0        0 2023-07-03 19:03:02.938199 excel2mssql-0.0.1/excel2mssql.egg-info/
--rw-rw-rw-   0        0        0     3403 2023-07-03 19:03:02.000000 excel2mssql-0.0.1/excel2mssql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-07-03 19:03:02.000000 excel2mssql-0.0.1/excel2mssql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 19:03:02.000000 excel2mssql-0.0.1/excel2mssql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-03 19:03:02.000000 excel2mssql-0.0.1/excel2mssql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-03 19:03:02.000000 excel2mssql-0.0.1/excel2mssql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 19:03:02.947940 excel2mssql-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-07-03 19:02:20.000000 excel2mssql-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 19:50:25.601064 excel2mssql-0.0.2/
+-rw-rw-rw-   0        0        0     1099 2023-07-03 13:35:18.000000 excel2mssql-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3417 2023-07-03 19:50:25.595142 excel2mssql-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2923 2023-07-03 19:49:44.000000 excel2mssql-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 19:50:25.541020 excel2mssql-0.0.2/excel2mssql/
+-rw-rw-rw-   0        0        0        0 2023-07-03 13:42:30.000000 excel2mssql-0.0.2/excel2mssql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 19:50:25.586142 excel2mssql-0.0.2/excel2mssql/data/
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:22:52.000000 excel2mssql-0.0.2/excel2mssql/data/__init__.py
+-rw-rw-rw-   0        0        0      141 2023-07-03 16:26:15.000000 excel2mssql-0.0.2/excel2mssql/data/constants.py
+-rw-rw-rw-   0        0        0     8002 2023-07-03 17:50:18.000000 excel2mssql-0.0.2/excel2mssql/worker.py
+drwxrwxrwx   0        0        0        0 2023-07-03 19:50:25.576609 excel2mssql-0.0.2/excel2mssql.egg-info/
+-rw-rw-rw-   0        0        0     3417 2023-07-03 19:50:25.000000 excel2mssql-0.0.2/excel2mssql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-07-03 19:50:25.000000 excel2mssql-0.0.2/excel2mssql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 19:50:25.000000 excel2mssql-0.0.2/excel2mssql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-03 19:50:25.000000 excel2mssql-0.0.2/excel2mssql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-03 19:50:25.000000 excel2mssql-0.0.2/excel2mssql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 19:50:25.601064 excel2mssql-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-07-03 19:45:49.000000 excel2mssql-0.0.2/setup.py
```

### Comparing `excel2mssql-0.0.1/LICENSE` & `excel2mssql-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `excel2mssql-0.0.1/PKG-INFO` & `excel2mssql-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel2mssql
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to insert data from Excel or CSV to MSSQL
 Home-page: https://github.com/josehenriqueroveda/excel-to-mssql
 Author: Jose Henrique Roveda
 Author-email: josehenriqueroveda.dev@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 ```
 
 ## Usage
 ### CsvToMssql
 To use `CsvToMssql`, you need to create an instance of the class and pass in the path to the CSV file, the name or IP address of the SQL Server, the name of the database to connect to, the name of the table to insert the data into, and the username and password to use for authentication.
 
 ```python
-from excel2mssql import CsvToMssql
+from excel2mssql.worker import CsvToMssql
 
 csv_path = "path/to/csv/file.csv"
 
 # This is just an example, preferably you would store these in environment variables
 server = "localhost"
 database = "mydatabase"
 schema = "myschema"
@@ -52,15 +52,15 @@
 csv_to_mssql.csv_to_mssql(columns=columns, sep=",", encoding="utf-8", action="replace")
 ```
 
 ### ExcelToMssql
 To use `ExcelToMssql`, you need to create an instance of the class and pass in the path to the Excel file, the name or IP address of the SQL Server, the name of the database to connect to, the name of the table to insert the data into, and the username and password to use for authentication.
 
 ```python
-from excel2mssql import ExcelToMssql
+from excel2mssql.worker import ExcelToMssql
 
 excel_path = "path/to/excel/file.xlsx"
 
 # This is just an example, preferably you would store these in environment variables
 server = "localhost"
 database = "mydatabase"
 schema = "myschema"
```

### Comparing `excel2mssql-0.0.1/README.md` & `excel2mssql-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```
 
 ## Usage
 ### CsvToMssql
 To use `CsvToMssql`, you need to create an instance of the class and pass in the path to the CSV file, the name or IP address of the SQL Server, the name of the database to connect to, the name of the table to insert the data into, and the username and password to use for authentication.
 
 ```python
-from excel2mssql import CsvToMssql
+from excel2mssql.worker import CsvToMssql
 
 csv_path = "path/to/csv/file.csv"
 
 # This is just an example, preferably you would store these in environment variables
 server = "localhost"
 database = "mydatabase"
 schema = "myschema"
@@ -38,15 +38,15 @@
 csv_to_mssql.csv_to_mssql(columns=columns, sep=",", encoding="utf-8", action="replace")
 ```
 
 ### ExcelToMssql
 To use `ExcelToMssql`, you need to create an instance of the class and pass in the path to the Excel file, the name or IP address of the SQL Server, the name of the database to connect to, the name of the table to insert the data into, and the username and password to use for authentication.
 
 ```python
-from excel2mssql import ExcelToMssql
+from excel2mssql.worker import ExcelToMssql
 
 excel_path = "path/to/excel/file.xlsx"
 
 # This is just an example, preferably you would store these in environment variables
 server = "localhost"
 database = "mydatabase"
 schema = "myschema"
```

### Comparing `excel2mssql-0.0.1/app/excel2mssql/excel2mssql.py` & `excel2mssql-0.0.2/excel2mssql/worker.py`

 * *Files identical despite different names*

### Comparing `excel2mssql-0.0.1/excel2mssql.egg-info/PKG-INFO` & `excel2mssql-0.0.2/excel2mssql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel2mssql
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to insert data from Excel or CSV to MSSQL
 Home-page: https://github.com/josehenriqueroveda/excel-to-mssql
 Author: Jose Henrique Roveda
 Author-email: josehenriqueroveda.dev@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 ```
 
 ## Usage
 ### CsvToMssql
 To use `CsvToMssql`, you need to create an instance of the class and pass in the path to the CSV file, the name or IP address of the SQL Server, the name of the database to connect to, the name of the table to insert the data into, and the username and password to use for authentication.
 
 ```python
-from excel2mssql import CsvToMssql
+from excel2mssql.worker import CsvToMssql
 
 csv_path = "path/to/csv/file.csv"
 
 # This is just an example, preferably you would store these in environment variables
 server = "localhost"
 database = "mydatabase"
 schema = "myschema"
@@ -52,15 +52,15 @@
 csv_to_mssql.csv_to_mssql(columns=columns, sep=",", encoding="utf-8", action="replace")
 ```
 
 ### ExcelToMssql
 To use `ExcelToMssql`, you need to create an instance of the class and pass in the path to the Excel file, the name or IP address of the SQL Server, the name of the database to connect to, the name of the table to insert the data into, and the username and password to use for authentication.
 
 ```python
-from excel2mssql import ExcelToMssql
+from excel2mssql.worker import ExcelToMssql
 
 excel_path = "path/to/excel/file.xlsx"
 
 # This is just an example, preferably you would store these in environment variables
 server = "localhost"
 database = "mydatabase"
 schema = "myschema"
```

### Comparing `excel2mssql-0.0.1/setup.py` & `excel2mssql-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name="excel2mssql",
-    version="0.0.1",
+    version="0.0.2",
     description="A package to insert data from Excel or CSV to MSSQL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jose Henrique Roveda",
     author_email="josehenriqueroveda.dev@gmail.com",
     url="https://github.com/josehenriqueroveda/excel-to-mssql",
     packages=find_packages(),
```


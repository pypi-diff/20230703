# Comparing `tmp/sensitibot-1.1.0.tar.gz` & `tmp/sensitibot-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensitibot-1.1.0.tar", max compression
+gzip compressed data, was "sensitibot-1.1.1.tar", max compression
```

## Comparing `sensitibot-1.1.0.tar` & `sensitibot-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0        0 2023-06-12 19:53:18.779840 sensitibot-1.1.0/cleaner/__init__.py
--rw-r--r--   0        0        0     2466 2023-06-12 19:54:58.518829 sensitibot-1.1.0/cleaner/access_cleaner.py
--rw-r--r--   0        0        0     3396 2023-06-25 16:06:00.250762 sensitibot-1.1.0/cleaner/cleaner.py
--rw-r--r--   0        0        0     1176 2023-06-12 19:53:18.780838 sensitibot-1.1.0/cleaner/csv_cleaner.py
--rw-r--r--   0        0        0     1691 2023-06-12 19:53:18.781837 sensitibot-1.1.0/cleaner/excel_cleaner.py
--rw-r--r--   0        0        0     1343 2023-06-12 19:54:58.519830 sensitibot-1.1.0/cleaner/json_cleaner.py
--rw-r--r--   0        0        0     1948 2023-06-12 19:54:58.519830 sensitibot-1.1.0/cleaner/show_matches.py
--rw-r--r--   0        0        0     1177 2023-06-12 19:53:18.782840 sensitibot-1.1.0/cleaner/tsv_cleaner.py
--rw-r--r--   0        0        0        0 2023-06-12 19:53:18.782840 sensitibot-1.1.0/github/__init__.py
--rw-r--r--   0        0        0     8713 2023-06-25 15:30:27.861844 sensitibot-1.1.0/github/github.py
--rw-r--r--   0        0        0        0 2023-06-12 19:53:18.783839 sensitibot-1.1.0/local/__init__.py
--rw-r--r--   0        0        0     1383 2023-06-25 15:30:40.284141 sensitibot-1.1.0/local/local.py
--rw-r--r--   0        0        0      997 2023-06-27 15:38:05.601306 sensitibot-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-12 19:53:18.787841 sensitibot-1.1.0/reader/__init__.py
--rw-r--r--   0        0        0     4365 2023-06-12 19:54:58.523829 sensitibot-1.1.0/reader/access_reader.py
--rw-r--r--   0        0        0     1701 2023-06-12 19:53:18.788840 sensitibot-1.1.0/reader/columns_reader.py
--rw-r--r--   0        0        0     1286 2023-06-12 19:53:18.789839 sensitibot-1.1.0/reader/csv_reader.py
--rw-r--r--   0        0        0     3038 2023-06-12 19:53:18.790878 sensitibot-1.1.0/reader/excel_reader.py
--rw-r--r--   0        0        0     1272 2023-06-12 19:53:18.790878 sensitibot-1.1.0/reader/headers_reader.py
--rw-r--r--   0        0        0     1333 2023-06-12 19:54:58.523829 sensitibot-1.1.0/reader/json_reader.py
--rw-r--r--   0        0        0     3458 2023-06-25 16:06:25.804932 sensitibot-1.1.0/reader/reader.py
--rw-r--r--   0        0        0     1286 2023-06-12 19:53:18.791838 sensitibot-1.1.0/reader/tsv_reader.py
--rw-r--r--   0        0        0      628 2023-06-22 19:08:34.082525 sensitibot-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-12 19:53:18.792844 sensitibot-1.1.0/renderer/__init__.py
--rw-r--r--   0        0        0     1584 2023-06-22 19:19:21.522620 sensitibot-1.1.0/renderer/renderer.py
--rw-r--r--   0        0        0        0 2023-06-12 19:53:18.794840 sensitibot-1.1.0/sensitibot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 19:53:18.794840 sensitibot-1.1.0/sensitibot/__main__.py
--rw-r--r--   0        0        0     1084 2023-06-12 19:54:58.527831 sensitibot-1.1.0/sensitibot/custom_formatters.py
--rw-r--r--   0        0        0     2595 2023-06-22 19:08:34.146146 sensitibot-1.1.0/sensitibot/parser.py
--rw-r--r--   0        0        0     1211 2023-06-22 19:08:34.160161 sensitibot-1.1.0/sensitibot/sensitibot.py
--rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 sensitibot-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.779840 sensitibot-1.1.1/cleaner/__init__.py
+-rw-r--r--   0        0        0     2466 2023-06-12 19:54:58.518829 sensitibot-1.1.1/cleaner/access_cleaner.py
+-rw-r--r--   0        0        0     3500 2023-07-03 02:58:53.095501 sensitibot-1.1.1/cleaner/cleaner.py
+-rw-r--r--   0        0        0     1176 2023-06-12 19:53:18.780838 sensitibot-1.1.1/cleaner/csv_cleaner.py
+-rw-r--r--   0        0        0     1775 2023-07-03 02:47:40.820598 sensitibot-1.1.1/cleaner/excel_cleaner.py
+-rw-r--r--   0        0        0     1343 2023-06-12 19:54:58.519830 sensitibot-1.1.1/cleaner/json_cleaner.py
+-rw-r--r--   0        0        0     1948 2023-06-12 19:54:58.519830 sensitibot-1.1.1/cleaner/show_matches.py
+-rw-r--r--   0        0        0     1177 2023-06-12 19:53:18.782840 sensitibot-1.1.1/cleaner/tsv_cleaner.py
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.782840 sensitibot-1.1.1/github/__init__.py
+-rw-r--r--   0        0        0     8713 2023-06-25 15:30:27.861844 sensitibot-1.1.1/github/github.py
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.783839 sensitibot-1.1.1/local/__init__.py
+-rw-r--r--   0        0        0     1383 2023-06-25 15:30:40.284141 sensitibot-1.1.1/local/local.py
+-rw-r--r--   0        0        0      997 2023-07-03 02:53:17.041108 sensitibot-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.787841 sensitibot-1.1.1/reader/__init__.py
+-rw-r--r--   0        0        0     4365 2023-06-12 19:54:58.523829 sensitibot-1.1.1/reader/access_reader.py
+-rw-r--r--   0        0        0     1701 2023-06-12 19:53:18.788840 sensitibot-1.1.1/reader/columns_reader.py
+-rw-r--r--   0        0        0     1286 2023-06-12 19:53:18.789839 sensitibot-1.1.1/reader/csv_reader.py
+-rw-r--r--   0        0        0     3038 2023-06-12 19:53:18.790878 sensitibot-1.1.1/reader/excel_reader.py
+-rw-r--r--   0        0        0     1272 2023-06-12 19:53:18.790878 sensitibot-1.1.1/reader/headers_reader.py
+-rw-r--r--   0        0        0     1333 2023-06-12 19:54:58.523829 sensitibot-1.1.1/reader/json_reader.py
+-rw-r--r--   0        0        0     3458 2023-06-25 16:06:25.804932 sensitibot-1.1.1/reader/reader.py
+-rw-r--r--   0        0        0     1286 2023-06-12 19:53:18.791838 sensitibot-1.1.1/reader/tsv_reader.py
+-rw-r--r--   0        0        0      628 2023-06-22 19:08:34.082525 sensitibot-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.792844 sensitibot-1.1.1/renderer/__init__.py
+-rw-r--r--   0        0        0     1584 2023-06-22 19:19:21.522620 sensitibot-1.1.1/renderer/renderer.py
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.794840 sensitibot-1.1.1/sensitibot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.794840 sensitibot-1.1.1/sensitibot/__main__.py
+-rw-r--r--   0        0        0     1084 2023-06-12 19:54:58.527831 sensitibot-1.1.1/sensitibot/custom_formatters.py
+-rw-r--r--   0        0        0     2595 2023-06-22 19:08:34.146146 sensitibot-1.1.1/sensitibot/parser.py
+-rw-r--r--   0        0        0     1211 2023-06-22 19:08:34.160161 sensitibot-1.1.1/sensitibot/sensitibot.py
+-rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 sensitibot-1.1.1/PKG-INFO
```

### Comparing `sensitibot-1.1.0/cleaner/access_cleaner.py` & `sensitibot-1.1.1/cleaner/access_cleaner.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/cleaner/cleaner.py` & `sensitibot-1.1.1/cleaner/cleaner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from cleaner import (csv_cleaner, excel_cleaner, json_cleaner, show_matches,
                      tsv_cleaner)
 
 
 def process_cleaner(files):
+    if "files" not in files["repositories"][0]:
+        print("\nNo files to clean.")
+        return
     generate_clean_files = input(
         "\nDo you want to generate clean files? (yes/no): ")
     while generate_clean_files.lower() not in ("yes", "no"):
         generate_clean_files = input("Please enter either 'yes' or 'no': ")
     if generate_clean_files.lower() == "yes":
         clean_files(files)
```

### Comparing `sensitibot-1.1.0/cleaner/csv_cleaner.py` & `sensitibot-1.1.1/cleaner/csv_cleaner.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/cleaner/excel_cleaner.py` & `sensitibot-1.1.1/cleaner/excel_cleaner.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,15 @@
     try:
         data = pd.ExcelFile(filename, engine='openpyxl')
     except Exception as e:
         error = {"file": filename, "error": str(e)}
 
     base_filename, extension = os.path.splitext(filename)
 
-    if not replace_file:
-        base_filename = base_filename + "_clean"
+    base_filename = base_filename + "_clean"
 
     new_filename = base_filename + extension
 
     writer = pd.ExcelWriter(new_filename, engine='xlsxwriter')
 
     for sheet_name in data.sheet_names:
         sheet_data = data.parse(sheet_name, dtype=str)
@@ -48,7 +47,12 @@
             for column in columns:
                 if column in positive_headers or column in list(positive_columns.keys()):
                     sheet_data = sheet_data.drop(column, axis=1)
 
         sheet_data.to_excel(writer, sheet_name=sheet_name, index=False)
 
     writer.close()
+    data.close()
+
+    if replace_file:
+        os.remove(filename)
+        os.rename(new_filename, filename)
```

### Comparing `sensitibot-1.1.0/cleaner/json_cleaner.py` & `sensitibot-1.1.1/cleaner/json_cleaner.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/cleaner/show_matches.py` & `sensitibot-1.1.1/cleaner/show_matches.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/cleaner/tsv_cleaner.py` & `sensitibot-1.1.1/cleaner/tsv_cleaner.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/github/github.py` & `sensitibot-1.1.1/github/github.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/local/local.py` & `sensitibot-1.1.1/local/local.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/pyproject.toml` & `sensitibot-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SensitiBot"
-version = "1.1.0"
+version = "1.1.1"
 description = "A Python bot to detect data leaks on public repositories"
 readme = "README.md"
 authors = ["José Manuel Martín Luque <josemanuelmartinluque@outlook.com>"]
 packages = [
     { include = "sensitibot" },
     { include = "local" },
     { include = "github" },
```

### Comparing `sensitibot-1.1.0/reader/access_reader.py` & `sensitibot-1.1.1/reader/access_reader.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/reader/columns_reader.py` & `sensitibot-1.1.1/reader/columns_reader.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/reader/csv_reader.py` & `sensitibot-1.1.1/reader/csv_reader.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/reader/excel_reader.py` & `sensitibot-1.1.1/reader/excel_reader.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/reader/headers_reader.py` & `sensitibot-1.1.1/reader/headers_reader.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/reader/json_reader.py` & `sensitibot-1.1.1/reader/json_reader.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/reader/reader.py` & `sensitibot-1.1.1/reader/reader.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/reader/tsv_reader.py` & `sensitibot-1.1.1/reader/tsv_reader.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/README.md` & `sensitibot-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/renderer/renderer.py` & `sensitibot-1.1.1/renderer/renderer.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/sensitibot/custom_formatters.py` & `sensitibot-1.1.1/sensitibot/custom_formatters.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/sensitibot/parser.py` & `sensitibot-1.1.1/sensitibot/parser.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/sensitibot/sensitibot.py` & `sensitibot-1.1.1/sensitibot/sensitibot.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.1.0/PKG-INFO` & `sensitibot-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensitibot
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python bot to detect data leaks on public repositories
 Author: José Manuel Martín Luque
 Author-email: josemanuelmartinluque@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: XlsxWriter (>=3.1.0,<4.0.0)
```


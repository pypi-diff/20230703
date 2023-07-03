# Comparing `tmp/spark_acl_tools-0.2.0.tar.gz` & `tmp/spark_acl_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_acl_tools-0.2.0.tar", last modified: Sun Jun 25 20:28:44 2023, max compression
+gzip compressed data, was "spark_acl_tools-0.3.0.tar", last modified: Mon Jul  3 10:08:17 2023, max compression
```

## Comparing `spark_acl_tools-0.2.0.tar` & `spark_acl_tools-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 20:28:44.156263 spark_acl_tools-0.2.0/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_acl_tools-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       41 2023-06-25 06:14:15.000000 spark_acl_tools-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5704 2023-06-25 20:28:44.156263 spark_acl_tools-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4949 2023-06-25 09:26:52.000000 spark_acl_tools-0.2.0/README.md
--rw-rw-rw-   0        0        0      633 2023-06-25 06:52:01.000000 spark_acl_tools-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-25 20:28:44.158264 spark_acl_tools-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-06-25 20:28:28.000000 spark_acl_tools-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:28:44.114251 spark_acl_tools-0.2.0/spark_acl_tools/
--rw-rw-rw-   0        0        0     1428 2023-06-25 08:40:18.000000 spark_acl_tools-0.2.0/spark_acl_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:28:44.134255 spark_acl_tools-0.2.0/spark_acl_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_acl_tools-0.2.0/spark_acl_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    19184 2023-06-25 20:28:12.000000 spark_acl_tools-0.2.0/spark_acl_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:28:44.144257 spark_acl_tools-0.2.0/spark_acl_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_acl_tools-0.2.0/spark_acl_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_acl_tools-0.2.0/spark_acl_tools/utils/color.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:28:44.155263 spark_acl_tools-0.2.0/spark_acl_tools/utils/files/
--rw-rw-rw-   0        0        0    24641 2023-06-24 17:38:32.000000 spark_acl_tools-0.2.0/spark_acl_tools/utils/files/acl.xlsx
--rw-rw-rw-   0        0        0     5750 2023-06-25 06:08:18.000000 spark_acl_tools-0.2.0/spark_acl_tools/utils/files/ns.csv
-drwxrwxrwx   0        0        0        0 2023-06-25 20:28:44.133255 spark_acl_tools-0.2.0/spark_acl_tools.egg-info/
--rw-rw-rw-   0        0        0     5704 2023-06-25 20:28:44.000000 spark_acl_tools-0.2.0/spark_acl_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2023-06-25 20:28:44.000000 spark_acl_tools-0.2.0/spark_acl_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 20:28:44.000000 spark_acl_tools-0.2.0/spark_acl_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2023-06-25 20:28:44.000000 spark_acl_tools-0.2.0/spark_acl_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-25 20:28:44.000000 spark_acl_tools-0.2.0/spark_acl_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 10:08:17.898126 spark_acl_tools-0.3.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_acl_tools-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       41 2023-06-25 06:14:15.000000 spark_acl_tools-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5700 2023-07-03 10:08:17.898126 spark_acl_tools-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4949 2023-06-25 09:26:52.000000 spark_acl_tools-0.3.0/README.md
+-rw-rw-rw-   0        0        0      632 2023-07-03 10:07:40.000000 spark_acl_tools-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-03 10:08:17.899126 spark_acl_tools-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1156 2023-07-03 10:08:05.000000 spark_acl_tools-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:08:17.852641 spark_acl_tools-0.3.0/spark_acl_tools/
+-rw-rw-rw-   0        0        0     1428 2023-06-25 08:40:18.000000 spark_acl_tools-0.3.0/spark_acl_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:08:17.878649 spark_acl_tools-0.3.0/spark_acl_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_acl_tools-0.3.0/spark_acl_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    19886 2023-06-26 12:03:41.000000 spark_acl_tools-0.3.0/spark_acl_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:08:17.887651 spark_acl_tools-0.3.0/spark_acl_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_acl_tools-0.3.0/spark_acl_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_acl_tools-0.3.0/spark_acl_tools/utils/color.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:08:17.897126 spark_acl_tools-0.3.0/spark_acl_tools/utils/files/
+-rw-rw-rw-   0        0        0    24641 2023-06-24 17:38:32.000000 spark_acl_tools-0.3.0/spark_acl_tools/utils/files/acl.xlsx
+-rw-rw-rw-   0        0        0     5750 2023-06-25 06:08:18.000000 spark_acl_tools-0.3.0/spark_acl_tools/utils/files/ns.csv
+drwxrwxrwx   0        0        0        0 2023-07-03 10:08:17.871649 spark_acl_tools-0.3.0/spark_acl_tools.egg-info/
+-rw-rw-rw-   0        0        0     5700 2023-07-03 10:08:17.000000 spark_acl_tools-0.3.0/spark_acl_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2023-07-03 10:08:17.000000 spark_acl_tools-0.3.0/spark_acl_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 10:08:17.000000 spark_acl_tools-0.3.0/spark_acl_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-07-03 10:08:17.000000 spark_acl_tools-0.3.0/spark_acl_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-03 10:08:17.000000 spark_acl_tools-0.3.0/spark_acl_tools.egg-info/top_level.txt
```

### Comparing `spark_acl_tools-0.2.0/LICENSE` & `spark_acl_tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_acl_tools-0.2.0/PKG-INFO` & `spark_acl_tools-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: spark_acl_tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: spark_acl_tools
-Home-page: https://github.com/jonaqp/spark_datax_tools/
+Home-page: https://github.com/jonaqp/spark_acl_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/jonaqp/spark_datax_tools/archive/main.zip
+Download-URL: https://github.com/jonaqp/spark_acl_tools/archive/main.zip
 Keywords: spark,datax,schema
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `spark_acl_tools-0.2.0/README.md` & `spark_acl_tools-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_acl_tools-0.2.0/pyproject.toml` & `spark_acl_tools-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 pandas = "^2.0.1"
 numpy = "^1.24.3"
 pyspark = "3.1.1"
 setuptools = "58.2.0"
 findspark = "^2.0.1"
 pyarrow = "^12.0.0"
 spark-dataframe-tools = "^0.2.0"
-prettytable = "^3.7.0"
+prettytable = "3.8.0"
 color-tools = "^0.0.2"
 openpyxl = "^3.1.2"
 
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^4.0.0"
 twine = "^4.0.2"
```

### Comparing `spark_acl_tools-0.2.0/setup.py` & `spark_acl_tools-0.3.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_acl_tools',
     packages=find_packages(),
-    version='0.2.0',
+    version='0.3.0',
     description='spark_acl_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
-    url='https://github.com/jonaqp/spark_datax_tools/',
-    download_url='https://github.com/jonaqp/spark_datax_tools/archive/main.zip',
+    url='https://github.com/jonaqp/spark_acl_tools/',
+    download_url='https://github.com/jonaqp/spark_acl_tools/archive/main.zip',
     keywords=['spark', 'datax', 'schema'],
     install_requires=open(os.path.join(setuppath, 'requirements.txt')).read().splitlines(),
     dependency_links=[],
     include_package_data=True,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

### Comparing `spark_acl_tools-0.2.0/spark_acl_tools/__init__.py` & `spark_acl_tools-0.3.0/spark_acl_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_acl_tools-0.2.0/spark_acl_tools/functions/generator.py` & `spark_acl_tools-0.3.0/spark_acl_tools/functions/generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,14 +104,16 @@
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_INGESTA_MASTER", col=x["Path"], uuaa_master=uuaa_master, ns=ns),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
     path_directory = os.path.join("DIRECTORY_ACL", "ACL_PROJECT_INGESTA_MASTER", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
+    if is_windows:
+        path_filename = path_filename.replace("\\", "/")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
 
@@ -142,14 +144,16 @@
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_INGESTA_RAW", col=x["Path"], uuaa_raw=uuaa_raw, ns=ns),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
     path_directory = os.path.join("DIRECTORY_ACL", "ACL_PROJECT_INGESTA_RAW", uuaa_raw)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
+    if is_windows:
+        path_filename = path_filename.replace("\\", "/")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_raw}'))
     print(f'create file for acl: {path_filename}')
 
@@ -183,14 +187,16 @@
         lambda x: get_replace_value(acl_name="ACL_PROCESAMIENTO_MASTER", col=x["Path"],
                                     uuaa_master=uuaa_master, ns=ns),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
     path_directory = os.path.join("DIRECTORY_ACL", "ACL_PROJECT_PROCESAMIENTO", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
+    if is_windows:
+        path_filename = path_filename.replace("\\", "/")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
 
@@ -227,14 +233,16 @@
         lambda x: get_replace_value(acl_name="ACL_RAW", col=x["Path"], uuaa_master=uuaa_master,
                                     uuaa_raw=uuaa_raw, ns=ns),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
     path_directory = os.path.join("DIRECTORY_ACL", "ACL_RUTA_RAW", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
+    if is_windows:
+        path_filename = path_filename.replace("\\", "/")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
 
@@ -271,14 +279,16 @@
         lambda x: get_replace_value(acl_name="ACL_STAGING", col=x["Path"], uuaa_master=uuaa_master,
                                     uuaa_staging=uuaa_staging, ns=ns),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
     path_directory = os.path.join("DIRECTORY_ACL", "ACL_RUTA_STAGING", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
+    if is_windows:
+        path_filename = path_filename.replace("\\", "/")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
 
@@ -315,14 +325,16 @@
         lambda x: get_replace_value(acl_name="ACL_READ", col=x["Path"], uuaa_master=uuaa_master,
                                     uuaa_master_read=uuaa_master_read, ns=ns),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
     path_directory = os.path.join("DIRECTORY_ACL", "ACL_RUTA_READ", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
+    if is_windows:
+        path_filename = path_filename.replace("\\", "/")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
 
@@ -352,14 +364,16 @@
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_MONITORING", col=x["Path"], uuaa_master=uuaa_master),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
     path_directory = os.path.join("DIRECTORY_ACL", "ACL_RUTA_ARGOS", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
+    if is_windows:
+        path_filename = path_filename.replace("\\", "/")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
 
@@ -389,14 +403,16 @@
     data["Path"] = data.apply(
         lambda x: get_replace_value(acl_name="ACL_DATAPROC", col=x["Path"], uuaa_master=uuaa_master),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
     path_directory = os.path.join("DIRECTORY_ACL", "ACL_RUTA_DATAPROC", uuaa_master)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
+    if is_windows:
+        path_filename = path_filename.replace("\\", "/")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_master}'))
     print(f'create file for acl: {path_filename}')
 
@@ -430,13 +446,15 @@
         lambda x: get_replace_value(acl_name="ACL_SANDBOX", col=x["Path"],
                                     uuaa_sandbox=uuaa_sandbox, uuaa_master=uuaa_master),
         axis=1)
     data = data.drop(columns=['ACL_TYPE'])
 
     path_directory = os.path.join("DIRECTORY_ACL", "ACL_RUTA_SANDBOXLIVE", uuaa_sandbox)
     path_filename = os.path.join(path_directory, f"{sheet_name}- PE_UsuarioGrupo_DATASD-{nro_ticket}.xlsx")
+    if is_windows:
+        path_filename = path_filename.replace("\\", "/")
     if not os.path.exists(path_directory):
         os.makedirs(path_directory)
     data.to_excel(path_filename, index=False, sheet_name='ACLs')
 
     print(get_color_b(f'GENERATED ACL UUAA: {uuaa_sandbox}'))
     print(f'create file for acl: {path_filename}')
```

### Comparing `spark_acl_tools-0.2.0/spark_acl_tools/utils/files/acl.xlsx` & `spark_acl_tools-0.3.0/spark_acl_tools/utils/files/acl.xlsx`

 * *Files identical despite different names*

### Comparing `spark_acl_tools-0.2.0/spark_acl_tools/utils/files/ns.csv` & `spark_acl_tools-0.3.0/spark_acl_tools/utils/files/ns.csv`

 * *Files identical despite different names*

### Comparing `spark_acl_tools-0.2.0/spark_acl_tools.egg-info/PKG-INFO` & `spark_acl_tools-0.3.0/spark_acl_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: spark-acl-tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: spark_acl_tools
-Home-page: https://github.com/jonaqp/spark_datax_tools/
+Home-page: https://github.com/jonaqp/spark_acl_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/jonaqp/spark_datax_tools/archive/main.zip
+Download-URL: https://github.com/jonaqp/spark_acl_tools/archive/main.zip
 Keywords: spark,datax,schema
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
```


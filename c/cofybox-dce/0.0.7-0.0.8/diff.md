# Comparing `tmp/cofybox-dce-0.0.7.tar.gz` & `tmp/cofybox-dce-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cofybox-dce-0.0.7.tar", last modified: Mon Jul  3 11:02:21 2023, max compression
+gzip compressed data, was "cofybox-dce-0.0.8.tar", last modified: Mon Jul  3 13:46:58 2023, max compression
```

## Comparing `cofybox-dce-0.0.7.tar` & `cofybox-dce-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 11:02:21.545331 cofybox-dce-0.0.7/
--rw-r--r--   0 Jan        (504) staff       (20)     1055 2021-09-30 09:51:08.000000 cofybox-dce-0.0.7/LICENSE
--rw-r--r--   0 Jan        (504) staff       (20)      608 2023-07-03 11:02:21.545433 cofybox-dce-0.0.7/PKG-INFO
--rw-r--r--   0 Jan        (504) staff       (20)      101 2021-09-29 10:14:10.000000 cofybox-dce-0.0.7/README.md
--rw-r--r--   0 Jan        (504) staff       (20)      103 2021-09-30 09:40:16.000000 cofybox-dce-0.0.7/pyproject.toml
--rw-r--r--   0 Jan        (504) staff       (20)      705 2023-07-03 11:02:21.545864 cofybox-dce-0.0.7/setup.cfg
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 11:02:21.538311 cofybox-dce-0.0.7/src/
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 11:02:21.540756 cofybox-dce-0.0.7/src/cofybox_dce/
--rw-r--r--   0 Jan        (504) staff       (20)        0 2021-09-30 09:37:01.000000 cofybox-dce-0.0.7/src/cofybox_dce/__init__.py
--rw-r--r--   0 Jan        (504) staff       (20)      907 2023-07-03 09:07:57.000000 cofybox-dce-0.0.7/src/cofybox_dce/abstract.py
--rw-r--r--   0 Jan        (504) staff       (20)     2245 2023-07-03 10:58:34.000000 cofybox-dce-0.0.7/src/cofybox_dce/factory.py
--rw-r--r--   0 Jan        (504) staff       (20)      287 2023-06-29 14:21:07.000000 cofybox-dce-0.0.7/src/cofybox_dce/misc.py
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 11:02:21.543757 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/
--rw-r--r--   0 Jan        (504) staff       (20)      200 2023-07-03 10:59:02.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/__init__.py
--rw-r--r--   0 Jan        (504) staff       (20)     3354 2023-07-03 11:00:07.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/belgium.py
--rw-r--r--   0 Jan        (504) staff       (20)     2075 2023-07-03 10:52:16.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/france.py
--rw-r--r--   0 Jan        (504) staff       (20)     1949 2023-07-03 10:48:15.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/octopus.py
--rw-r--r--   0 Jan        (504) staff       (20)     4624 2023-07-03 10:53:33.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/octopus_outgoing_workaround.py
--rw-r--r--   0 Jan        (504) staff       (20)     1331 2023-07-03 10:48:03.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/pricing.py
--rw-r--r--   0 Jan        (504) staff       (20)     2271 2023-07-03 11:00:28.000000 cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/spain.py
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 11:02:21.541900 cofybox-dce-0.0.7/src/cofybox_dce.egg-info/
--rw-r--r--   0 Jan        (504) staff       (20)      608 2023-07-03 11:02:21.000000 cofybox-dce-0.0.7/src/cofybox_dce.egg-info/PKG-INFO
--rw-r--r--   0 Jan        (504) staff       (20)      790 2023-07-03 11:02:21.000000 cofybox-dce-0.0.7/src/cofybox_dce.egg-info/SOURCES.txt
--rw-r--r--   0 Jan        (504) staff       (20)        1 2023-07-03 11:02:21.000000 cofybox-dce-0.0.7/src/cofybox_dce.egg-info/dependency_links.txt
--rw-r--r--   0 Jan        (504) staff       (20)       51 2023-07-03 11:02:21.000000 cofybox-dce-0.0.7/src/cofybox_dce.egg-info/requires.txt
--rw-r--r--   0 Jan        (504) staff       (20)       12 2023-07-03 11:02:21.000000 cofybox-dce-0.0.7/src/cofybox_dce.egg-info/top_level.txt
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 11:02:21.545150 cofybox-dce-0.0.7/tests/
--rw-r--r--   0 Jan        (504) staff       (20)     1980 2023-07-03 10:48:18.000000 cofybox-dce-0.0.7/tests/test_belgium.py
--rw-r--r--   0 Jan        (504) staff       (20)     2522 2023-07-03 10:48:18.000000 cofybox-dce-0.0.7/tests/test_factory.py
--rw-r--r--   0 Jan        (504) staff       (20)     1119 2023-07-03 10:48:18.000000 cofybox-dce-0.0.7/tests/test_france.py
--rw-r--r--   0 Jan        (504) staff       (20)     2170 2023-07-03 10:48:18.000000 cofybox-dce-0.0.7/tests/test_octopus.py
--rw-r--r--   0 Jan        (504) staff       (20)     2087 2023-07-03 10:48:18.000000 cofybox-dce-0.0.7/tests/test_spain.py
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 13:46:58.802451 cofybox-dce-0.0.8/
+-rw-r--r--   0 Jan        (504) staff       (20)     1055 2021-09-30 09:51:08.000000 cofybox-dce-0.0.8/LICENSE
+-rw-r--r--   0 Jan        (504) staff       (20)      608 2023-07-03 13:46:58.802635 cofybox-dce-0.0.8/PKG-INFO
+-rw-r--r--   0 Jan        (504) staff       (20)      101 2021-09-29 10:14:10.000000 cofybox-dce-0.0.8/README.md
+-rw-r--r--   0 Jan        (504) staff       (20)      103 2021-09-30 09:40:16.000000 cofybox-dce-0.0.8/pyproject.toml
+-rw-r--r--   0 Jan        (504) staff       (20)      721 2023-07-03 13:46:58.803503 cofybox-dce-0.0.8/setup.cfg
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 13:46:58.794434 cofybox-dce-0.0.8/src/
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 13:46:58.797141 cofybox-dce-0.0.8/src/cofybox_dce/
+-rw-r--r--   0 Jan        (504) staff       (20)        0 2021-09-30 09:37:01.000000 cofybox-dce-0.0.8/src/cofybox_dce/__init__.py
+-rw-r--r--   0 Jan        (504) staff       (20)      907 2023-07-03 09:07:57.000000 cofybox-dce-0.0.8/src/cofybox_dce/abstract.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2245 2023-07-03 10:58:34.000000 cofybox-dce-0.0.8/src/cofybox_dce/factory.py
+-rw-r--r--   0 Jan        (504) staff       (20)      287 2023-06-29 14:21:07.000000 cofybox-dce-0.0.8/src/cofybox_dce/misc.py
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 13:46:58.799857 cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/
+-rw-r--r--   0 Jan        (504) staff       (20)      200 2023-07-03 10:59:02.000000 cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/__init__.py
+-rw-r--r--   0 Jan        (504) staff       (20)     3354 2023-07-03 11:00:07.000000 cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/belgium.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2076 2023-07-03 13:43:31.000000 cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/france.py
+-rw-r--r--   0 Jan        (504) staff       (20)     1949 2023-07-03 10:48:15.000000 cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/octopus.py
+-rw-r--r--   0 Jan        (504) staff       (20)     4624 2023-07-03 10:53:33.000000 cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/octopus_outgoing_workaround.py
+-rw-r--r--   0 Jan        (504) staff       (20)     1331 2023-07-03 10:48:03.000000 cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/pricing.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2271 2023-07-03 11:00:28.000000 cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/spain.py
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 13:46:58.798065 cofybox-dce-0.0.8/src/cofybox_dce.egg-info/
+-rw-r--r--   0 Jan        (504) staff       (20)      608 2023-07-03 13:46:58.000000 cofybox-dce-0.0.8/src/cofybox_dce.egg-info/PKG-INFO
+-rw-r--r--   0 Jan        (504) staff       (20)      790 2023-07-03 13:46:58.000000 cofybox-dce-0.0.8/src/cofybox_dce.egg-info/SOURCES.txt
+-rw-r--r--   0 Jan        (504) staff       (20)        1 2023-07-03 13:46:58.000000 cofybox-dce-0.0.8/src/cofybox_dce.egg-info/dependency_links.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       66 2023-07-03 13:46:58.000000 cofybox-dce-0.0.8/src/cofybox_dce.egg-info/requires.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       12 2023-07-03 13:46:58.000000 cofybox-dce-0.0.8/src/cofybox_dce.egg-info/top_level.txt
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-07-03 13:46:58.802147 cofybox-dce-0.0.8/tests/
+-rw-r--r--   0 Jan        (504) staff       (20)     1980 2023-07-03 10:48:18.000000 cofybox-dce-0.0.8/tests/test_belgium.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2522 2023-07-03 10:48:18.000000 cofybox-dce-0.0.8/tests/test_factory.py
+-rw-r--r--   0 Jan        (504) staff       (20)     1119 2023-07-03 10:48:18.000000 cofybox-dce-0.0.8/tests/test_france.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2170 2023-07-03 10:48:18.000000 cofybox-dce-0.0.8/tests/test_octopus.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2087 2023-07-03 10:48:18.000000 cofybox-dce-0.0.8/tests/test_spain.py
```

### Comparing `cofybox-dce-0.0.7/LICENSE` & `cofybox-dce-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/PKG-INFO` & `cofybox-dce-0.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofybox-dce
-Version: 0.0.7
+Version: 0.0.8
 Summary: COFYCloud Data Collector Engine python code
 Home-page: https://docs.cofybox.io
 Author: Jan Pecinovsky
 Author-email: jan@energieid.be
 Project-URL: Bug Tracker, https://gitlab.com/rescoopvpp/cofybox-dce/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cofybox-dce-0.0.7/setup.cfg` & `cofybox-dce-0.0.8/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cofybox-dce
-version = 0.0.7
+version = 0.0.8
 author = Jan Pecinovsky
 author_email = jan@energieid.be
 description = COFYCloud Data Collector Engine python code
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://docs.cofybox.io
 project_urls = 
@@ -19,14 +19,15 @@
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	pandas==1.4.0
 	octopusagile==0.0.6
 	entsoe-py==0.5.9
+	aiopvpc==4.2.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `cofybox-dce-0.0.7/src/cofybox_dce/abstract.py` & `cofybox-dce-0.0.8/src/cofybox_dce/abstract.py`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/src/cofybox_dce/factory.py` & `cofybox-dce-0.0.8/src/cofybox_dce/factory.py`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/belgium.py` & `cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/belgium.py`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/france.py` & `cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/france.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,10 +59,10 @@
 
         # Select tariff
         data_series = data_frame[self.tariff]
         data_series.rename("value_inc_vat", inplace=True)
         # From euro/MWh to eurocent/kWh
         data_series = data_series / 10
 
-        data_frame = pd.DataFrame(data_frame, columns=["value_inc_vat"])
+        data_frame = pd.DataFrame(data_series, columns=["value_inc_vat"])
         data_frame["Unit"] = self.unit
         return data_frame
```

### Comparing `cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/octopus.py` & `cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/octopus.py`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/octopus_outgoing_workaround.py` & `cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/octopus_outgoing_workaround.py`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/pricing.py` & `cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/pricing.py`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/src/cofybox_dce/pricing_collectors/spain.py` & `cofybox-dce-0.0.8/src/cofybox_dce/pricing_collectors/spain.py`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/src/cofybox_dce.egg-info/PKG-INFO` & `cofybox-dce-0.0.8/src/cofybox_dce.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofybox-dce
-Version: 0.0.7
+Version: 0.0.8
 Summary: COFYCloud Data Collector Engine python code
 Home-page: https://docs.cofybox.io
 Author: Jan Pecinovsky
 Author-email: jan@energieid.be
 Project-URL: Bug Tracker, https://gitlab.com/rescoopvpp/cofybox-dce/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cofybox-dce-0.0.7/src/cofybox_dce.egg-info/SOURCES.txt` & `cofybox-dce-0.0.8/src/cofybox_dce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/tests/test_belgium.py` & `cofybox-dce-0.0.8/tests/test_belgium.py`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/tests/test_factory.py` & `cofybox-dce-0.0.8/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/tests/test_france.py` & `cofybox-dce-0.0.8/tests/test_france.py`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/tests/test_octopus.py` & `cofybox-dce-0.0.8/tests/test_octopus.py`

 * *Files identical despite different names*

### Comparing `cofybox-dce-0.0.7/tests/test_spain.py` & `cofybox-dce-0.0.8/tests/test_spain.py`

 * *Files identical despite different names*


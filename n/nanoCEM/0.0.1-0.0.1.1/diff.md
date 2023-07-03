# Comparing `tmp/nanoCEM-0.0.1.tar.gz` & `tmp/nanoCEM-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.1.tar", last modified: Mon Jul  3 09:50:09 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.1.1.tar", last modified: Mon Jul  3 09:52:00 2023, max compression
```

## Comparing `nanoCEM-0.0.1.tar` & `nanoCEM-0.0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 09:50:09.723953 nanoCEM-0.0.1/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8935 2023-07-03 09:50:09.723953 nanoCEM-0.0.1/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8336 2023-07-03 09:49:00.000000 nanoCEM-0.0.1/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 09:50:09.723953 nanoCEM-0.0.1/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9323 2023-07-03 09:49:00.000000 nanoCEM-0.0.1/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7624 2023-07-03 09:49:00.000000 nanoCEM-0.0.1/nanoCEM/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1/nanoCEM/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7727 2023-06-26 15:00:04.000000 nanoCEM-0.0.1/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10594 2023-07-03 09:49:00.000000 nanoCEM-0.0.1/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13844 2023-07-03 09:49:00.000000 nanoCEM-0.0.1/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 09:50:09.723953 nanoCEM-0.0.1/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8935 2023-07-03 09:50:09.000000 nanoCEM-0.0.1/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-03 09:50:09.000000 nanoCEM-0.0.1/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-03 09:50:09.000000 nanoCEM-0.0.1/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-03 09:50:09.000000 nanoCEM-0.0.1/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-03 09:50:09.000000 nanoCEM-0.0.1/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-03 09:50:09.723953 nanoCEM-0.0.1/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1133 2023-07-03 09:50:08.000000 nanoCEM-0.0.1/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 09:52:00.000064 nanoCEM-0.0.1.1/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1.1/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8937 2023-07-03 09:52:00.000064 nanoCEM-0.0.1.1/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8336 2023-07-03 09:49:00.000000 nanoCEM-0.0.1.1/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 09:52:00.000064 nanoCEM-0.0.1.1/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9323 2023-07-03 09:49:00.000000 nanoCEM-0.0.1.1/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1.1/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1.1/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7624 2023-07-03 09:49:00.000000 nanoCEM-0.0.1.1/nanoCEM/current_events_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1.1/nanoCEM/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1.1/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7727 2023-06-26 15:00:04.000000 nanoCEM-0.0.1.1/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10594 2023-07-03 09:49:00.000000 nanoCEM-0.0.1.1/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13844 2023-07-03 09:49:00.000000 nanoCEM-0.0.1.1/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 09:52:00.000064 nanoCEM-0.0.1.1/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8937 2023-07-03 09:51:59.000000 nanoCEM-0.0.1.1/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-03 09:51:59.000000 nanoCEM-0.0.1.1/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-03 09:51:59.000000 nanoCEM-0.0.1.1/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-03 09:51:59.000000 nanoCEM-0.0.1.1/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-03 09:51:59.000000 nanoCEM-0.0.1.1/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-03 09:52:00.000064 nanoCEM-0.0.1.1/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1152 2023-07-03 09:51:59.000000 nanoCEM-0.0.1.1/setup.py
```

### Comparing `nanoCEM-0.0.1/LICENSE` & `nanoCEM-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1/PKG-INFO` & `nanoCEM-0.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanoCEM-0.0.1/README.md` & `nanoCEM-0.0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.1.1/nanoCEM/CE_magnifier_test.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1/nanoCEM/cem_utils.py` & `nanoCEM-0.0.1.1/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1/nanoCEM/current_events_magnifier.py` & `nanoCEM-0.0.1.1/nanoCEM/current_events_magnifier.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1/nanoCEM/extract_sub_fast5_from_bam.py` & `nanoCEM-0.0.1.1/nanoCEM/extract_sub_fast5_from_bam.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1/nanoCEM/normalization.py` & `nanoCEM-0.0.1.1/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1/nanoCEM/plot.py` & `nanoCEM-0.0.1.1/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.1.1/nanoCEM/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.1.1/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.1.1/nanoCEM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nanoCEM-0.0.1/setup.py` & `nanoCEM-0.0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.1",
+    version="0.0.1.1",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
@@ -26,9 +26,9 @@
         'pandas>=1.1.5',
         'plotnine>=0.8.0',
         'tqdm>=4.62.0',
         "pysam>=0.21.0",
         "pyslow5>=1.0.0",
         "vbz_h5py_plugin>=1.0.1"
     ],
-    scripts=['nanoCEM/nanoCEM.py','nanoCEM/extract_sub_fast5_from_bam.py']
+    scripts=['nanoCEM/current_events_magnifier.py','nanoCEM/extract_sub_fast5_from_bam.py']
 )
```


# Comparing `tmp/loreme-0.1.5.tar.gz` & `tmp/loreme-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loreme-0.1.5.tar", last modified: Thu Jun 15 18:32:59 2023, max compression
+gzip compressed data, was "loreme-0.1.6.tar", last modified: Mon Jul  3 21:34:03 2023, max compression
```

## Comparing `loreme-0.1.5.tar` & `loreme-0.1.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-15 18:32:59.075977 loreme-0.1.5/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-14 04:51:11.000000 loreme-0.1.5/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-06-15 18:32:59.075378 loreme-0.1.5/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4730 2023-06-14 04:58:53.000000 loreme-0.1.5/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-15 18:32:58.873185 loreme-0.1.5/loreme.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-06-15 18:32:58.000000 loreme-0.1.5/loreme.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-06-15 18:32:58.000000 loreme-0.1.5/loreme.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-06-15 18:32:58.000000 loreme-0.1.5/loreme.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-06-15 18:32:58.000000 loreme-0.1.5/loreme.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-06-15 18:32:58.000000 loreme-0.1.5/loreme.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-06-15 18:32:58.000000 loreme-0.1.5/loreme.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-06-14 05:34:47.000000 loreme-0.1.5/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-06-15 18:32:59.077527 loreme-0.1.5/setup.cfg
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-15 18:32:58.800566 loreme-0.1.5/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-15 18:32:59.074226 loreme-0.1.5/src/loreme/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1623 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/check_gpu_availability.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/check_tags.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/dorado.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6063 2023-06-15 18:05:04.000000 loreme-0.1.5/src/loreme/download.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3907 2023-06-15 18:07:10.000000 loreme-0.1.5/src/loreme/env.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/export_bedgraph.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/gene_body_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/intersect.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    37390 2023-06-15 18:22:10.000000 loreme-0.1.5/src/loreme/loreme.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5235 2023-06-14 05:31:42.000000 loreme-0.1.5/src/loreme/mean.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/merge.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/methylation_hist.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/modkit.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/parse_gff.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/pbcpg.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6531 2023-06-14 05:32:28.000000 loreme-0.1.5/src/loreme/plot.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2483 2023-06-14 05:33:30.000000 loreme-0.1.5/src/loreme/plot_bedtools.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/plot_genes.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/plot_repeats.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/promoter_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-06-14 05:34:58.000000 loreme-0.1.5/src/loreme/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-03 21:34:03.979321 loreme-0.1.6/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-14 04:51:11.000000 loreme-0.1.6/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-07-03 21:34:03.976913 loreme-0.1.6/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4730 2023-06-14 04:58:53.000000 loreme-0.1.6/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-03 21:34:03.938737 loreme-0.1.6/loreme.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-07-03 21:34:03.000000 loreme-0.1.6/loreme.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-07-03 21:34:03.000000 loreme-0.1.6/loreme.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-07-03 21:34:03.000000 loreme-0.1.6/loreme.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-07-03 21:34:03.000000 loreme-0.1.6/loreme.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-07-03 21:34:03.000000 loreme-0.1.6/loreme.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-07-03 21:34:03.000000 loreme-0.1.6/loreme.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-07-03 21:32:31.000000 loreme-0.1.6/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-07-03 21:34:03.979622 loreme-0.1.6/setup.cfg
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-03 21:34:03.927199 loreme-0.1.6/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-03 21:34:03.975839 loreme-0.1.6/src/loreme/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1623 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/check_gpu_availability.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/check_tags.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-07-03 21:29:32.000000 loreme-0.1.6/src/loreme/dorado.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6099 2023-07-03 21:25:22.000000 loreme-0.1.6/src/loreme/download.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3907 2023-06-26 22:02:40.000000 loreme-0.1.6/src/loreme/env.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/export_bedgraph.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/gene_body_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/intersect.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    37390 2023-06-26 22:03:44.000000 loreme-0.1.6/src/loreme/loreme.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5235 2023-06-14 05:31:42.000000 loreme-0.1.6/src/loreme/mean.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/merge.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/methylation_hist.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/modkit.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/parse_gff.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/pbcpg.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6531 2023-06-14 05:32:28.000000 loreme-0.1.6/src/loreme/plot.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2483 2023-06-14 05:33:30.000000 loreme-0.1.6/src/loreme/plot_bedtools.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/plot_genes.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/plot_repeats.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-14 04:51:11.000000 loreme-0.1.6/src/loreme/promoter_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-07-03 21:32:29.000000 loreme-0.1.6/src/loreme/version.py
```

### Comparing `loreme-0.1.5/LICENSE` & `loreme-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/PKG-INFO` & `loreme-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loreme
-Version: 0.1.5
+Version: 0.1.6
 Summary: Extract Methylation calls from ONT or PB long read data
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
 Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `loreme-0.1.5/README.md` & `loreme-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/loreme.egg-info/PKG-INFO` & `loreme-0.1.6/loreme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loreme
-Version: 0.1.5
+Version: 0.1.6
 Summary: Extract Methylation calls from ONT or PB long read data
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
 Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `loreme-0.1.5/loreme.egg-info/SOURCES.txt` & `loreme-0.1.6/loreme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/__init__.py` & `loreme-0.1.6/src/loreme/__init__.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/check_gpu_availability.py` & `loreme-0.1.6/src/loreme/check_gpu_availability.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/dorado.py` & `loreme-0.1.6/src/loreme/dorado.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/download.py` & `loreme-0.1.6/src/loreme/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import gzip
 import tarfile
 import subprocess
 import json
 from itertools import product
 from loreme.env import (PBCPG_URL, PBCPG_DIR, EXAMPLE_DATA_URLS, EXAMPLE_DATA_DIR, HG38_FTP,
                        HG38_GENOME_PATH, HG38_ANNOT_PATH, DORADO_DIR, DORADO_URL, DORADO_URL_024,
-                       DORADO_MODEL_DIR, DORADO_CONFIG, DORADO_PATH_024, MODKIT_URL, MODKIT_DIR)
+                       DORADO_MODEL_DIR, DORADO_CONFIG, DORADO_PATH, DORADO_PATH_024, MODKIT_URL,
+                       MODKIT_DIR)
 
 def download_pbcpg(directory: str = PBCPG_DIR):
     """Download pb-CpG-tools
 
     Parameters
     ----------
     directory : str
@@ -87,15 +88,15 @@
         Destination directory for dorado
     model_dir : str
         destination directory for dorado models
     """
 
     if pfm not in {'linux-x64', 'linux-arm64', 'osx-arm64', 'win64'}:
         raise RuntimeError('invalid platform choice')
-    dest_tarfile = os.path.join(directory, f'dorado-0.3.0-{pfm}.tar.gz')
+    dest_tarfile = os.path.join(directory, f'dorado-0.3.1-{pfm}.tar.gz')
     dest_tarfile_024 = os.path.join(directory, f'dorado-0.2.4-{pfm}.tar.gz')
     print(f'downloading to {dest_tarfile}')
     if os.path.exists(dest_tarfile):
         raise RuntimeError(f'a file already exists at {dest_tarfile}')
     http = urllib3.PoolManager()
     with http.request('GET', DORADO_URL[pfm], preload_content=False) as r, open(dest_tarfile, 'wb') as f:
         shutil.copyfileobj(r, f)
```

### Comparing `loreme-0.1.5/src/loreme/env.py` & `loreme-0.1.6/src/loreme/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,30 +27,30 @@
 if os.path.isfile(DORADO_CONFIG):
     with open(DORADO_CONFIG, 'r') as f:
         dorado_config = json.load(f)
 else:
     dorado_config = {}
 DORADO_PLATFORM = os.environ.get('LOREME_DORADO_PLATFORM', dorado_config.get('platform'))
 DORADO_PATH = {
-    'linux-x64': os.path.join(DORADO_DIR, 'dorado-0.3.0-linux-x64', 'bin', 'dorado'),
-    'linux-arm64': os.path.join(DORADO_DIR, 'dorado-0.3.0-linux-arm64', 'bin', 'dorado'),
-    'osx-arm64': os.path.join(DORADO_DIR, 'dorado-0.3.0-osx-arm64', 'bin', 'dorado'),
-    'win64': os.path.join(DORADO_DIR, 'dorado-0.3.0-win64', 'bin', 'dorado')
+    'linux-x64': os.path.join(DORADO_DIR, 'dorado-0.3.1-linux-x64', 'bin', 'dorado'),
+    'linux-arm64': os.path.join(DORADO_DIR, 'dorado-0.3.1-linux-arm64', 'bin', 'dorado'),
+    'osx-arm64': os.path.join(DORADO_DIR, 'dorado-0.3.1-osx-arm64', 'bin', 'dorado'),
+    'win64': os.path.join(DORADO_DIR, 'dorado-0.3.1-win64', 'bin', 'dorado')
 }
 DORADO_PATH_024 = {
     'linux-x64': os.path.join(DORADO_DIR, 'dorado-0.2.4-linux-x64', 'bin', 'dorado'),
     'linux-arm64': os.path.join(DORADO_DIR, 'dorado-0.2.4-linux-arm64', 'bin', 'dorado'),
     'osx-arm64': os.path.join(DORADO_DIR, 'dorado-0.2.4-osx-arm64', 'bin', 'dorado'),
     'win64': os.path.join(DORADO_DIR, 'dorado-0.2.4-win64', 'bin', 'dorado')
 }
 DORADO_URL = {
-    'linux-x64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.3.0-linux-x64.tar.gz',
-    'linux-arm64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.3.0-linux-arm64.tar.gz',
-    'osx-arm64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.3.0-osx-arm64.tar.gz',
-    'win64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.3.0-win64.zip'
+    'linux-x64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.3.1-linux-x64.tar.gz',
+    'linux-arm64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.3.1-linux-arm64.tar.gz',
+    'osx-arm64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.3.1-osx-arm64.tar.gz',
+    'win64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.3.1-win64.zip'
 }
 DORADO_URL_024 = {
     'linux-x64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.2.4-linux-x64.tar.gz',
     'linux-arm64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.2.4-linux-arm64.tar.gz',
     'osx-arm64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.2.4-osx-arm64.tar.gz',
     'win64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.2.4-win64.zip'
 }
```

### Comparing `loreme-0.1.5/src/loreme/export_bedgraph.py` & `loreme-0.1.6/src/loreme/export_bedgraph.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/gene_body_methylation.py` & `loreme-0.1.6/src/loreme/gene_body_methylation.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/intersect.py` & `loreme-0.1.6/src/loreme/intersect.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/loreme.py` & `loreme-0.1.6/src/loreme/loreme.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,22 +245,22 @@
     export_bedgraph(args.bedmethyl, chromosomes=args.chromosomes,
                     coverage=args.coverage)
 
 def clean(args):
     for root in args.dirs:
         for file in ('pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu.tar.gz',
                      'dorado-0.2.4-linux-x64.tar.gz',
-                     'dorado-0.3.0-linux-x64.tar.gz',
+                     'dorado-0.3.1-linux-x64.tar.gz',
                      'modkit_v0.1.8_centos7_x86_64.tar.gz',
                      'dorado-config.json'):
             if os.path.isfile(os.path.join(root, file)):
                 os.remove(os.path.join(root, file))
         for directory in ('pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu/',
                           f'dorado-0.2.4-{DORADO_PLATFORM}/',
-                          f'dorado-0.3.0-{DORADO_PLATFORM}/',
+                          f'dorado-0.3.1-{DORADO_PLATFORM}/',
                           'dna_r10.4.1_e8.2_260bps_fast@v4.1.0/',
                           'dna_r10.4.1_e8.2_260bps_hac@v4.1.0/',
                           'dna_r10.4.1_e8.2_260bps_sup@v4.1.0/',
                           'dna_r10.4.1_e8.2_400bps_fast@v4.1.0/',
                           'dna_r10.4.1_e8.2_400bps_hac@v4.1.0/',
                           'dna_r10.4.1_e8.2_400bps_sup@v4.1.0/',
                           'dna_r10.4.1_e8.2_260bps_fast@v4.1.0_5mCG_5hmCG@v2/',
```

### Comparing `loreme-0.1.5/src/loreme/mean.py` & `loreme-0.1.6/src/loreme/mean.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/merge.py` & `loreme-0.1.6/src/loreme/merge.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/methylation_hist.py` & `loreme-0.1.6/src/loreme/methylation_hist.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/parse_gff.py` & `loreme-0.1.6/src/loreme/parse_gff.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/pbcpg.py` & `loreme-0.1.6/src/loreme/pbcpg.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/plot.py` & `loreme-0.1.6/src/loreme/plot.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/plot_bedtools.py` & `loreme-0.1.6/src/loreme/plot_bedtools.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/plot_genes.py` & `loreme-0.1.6/src/loreme/plot_genes.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/plot_repeats.py` & `loreme-0.1.6/src/loreme/plot_repeats.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.5/src/loreme/promoter_methylation.py` & `loreme-0.1.6/src/loreme/promoter_methylation.py`

 * *Files identical despite different names*


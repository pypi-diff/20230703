# Comparing `tmp/splicekit-0.4.5.tar.gz` & `tmp/splicekit-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splicekit-0.4.5.tar", last modified: Fri Jun 30 14:19:58 2023, max compression
+gzip compressed data, was "splicekit-0.4.6.tar", last modified: Mon Jul  3 14:01:22 2023, max compression
```

## Comparing `splicekit-0.4.5.tar` & `splicekit-0.4.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.838842 splicekit-0.4.5/
--rw-rw-r--   0 rotg     (2023757) games       (20)    23915 2023-06-30 14:19:58.838444 splicekit-0.4.5/PKG-INFO
--rwxrwxr-x   0 rotg     (2023757) games       (20)    23517 2023-06-19 14:13:26.000000 splicekit-0.4.5/README.md
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-06-30 14:19:58.838946 splicekit-0.4.5/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)     1150 2023-06-12 17:55:56.000000 splicekit-0.4.5/setup.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.828846 splicekit-0.4.5/splicekit/
--rw-rw-r--   0 rotg     (2023757) games       (20)    13857 2023-06-08 07:08:02.000000 splicekit-0.4.5/splicekit/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.831055 splicekit-0.4.5/splicekit/clusterlogfc/
--rw-rw-r--   0 rotg     (2023757) games       (20)     5584 2023-05-05 11:49:03.000000 splicekit-0.4.5/splicekit/clusterlogfc/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.831627 splicekit-0.4.5/splicekit/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)      951 2023-06-07 13:26:10.000000 splicekit-0.4.5/splicekit/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.837498 splicekit-0.4.5/splicekit/core/
--rw-rw-r--   0 rotg     (2023757) games       (20)      119 2023-06-20 11:22:13.000000 splicekit-0.4.5/splicekit/core/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     6667 2023-05-05 06:13:11.000000 splicekit-0.4.5/splicekit/core/anchors.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    16752 2023-05-24 07:18:50.000000 splicekit-0.4.5/splicekit/core/annotation.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-01-31 12:27:24.000000 splicekit-0.4.5/splicekit/core/delta_dar.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     5407 2023-05-05 08:10:13.000000 splicekit-0.4.5/splicekit/core/exons.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)    30130 2023-06-30 14:19:04.000000 splicekit-0.4.5/splicekit/core/features.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     5662 2023-05-05 06:13:26.000000 splicekit-0.4.5/splicekit/core/genes.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1059 2023-06-07 14:32:33.000000 splicekit-0.4.5/splicekit/core/jbrowse2.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     9033 2023-06-08 11:52:41.000000 splicekit-0.4.5/splicekit/core/jbrowse2_create.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2948 2023-04-26 12:12:45.000000 splicekit-0.4.5/splicekit/core/juan.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    18195 2023-06-21 14:33:41.000000 splicekit-0.4.5/splicekit/core/junctions.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    37713 2023-05-04 06:56:59.000000 splicekit-0.4.5/splicekit/core/motifs.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1663 2023-05-02 18:35:35.000000 splicekit-0.4.5/splicekit/core/patterns.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2420 2023-05-03 10:54:22.000000 splicekit-0.4.5/splicekit/core/promisc.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     9045 2023-05-03 09:57:04.000000 splicekit-0.4.5/splicekit/core/report.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1527 2023-05-09 07:27:49.000000 splicekit-0.4.5/splicekit/folders.setup
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.837940 splicekit-0.4.5/splicekit/judge/
--rw-rw-r--   0 rotg     (2023757) games       (20)    26830 2023-06-08 11:49:08.000000 splicekit-0.4.5/splicekit/judge/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5402 2023-05-05 10:18:19.000000 splicekit-0.4.5/splicekit/splicecompare
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5117 2023-06-30 14:16:46.000000 splicekit-0.4.5/splicekit/splicekit
--rw-rw-r--   0 rotg     (2023757) games       (20)     1638 2023-06-06 07:56:19.000000 splicekit-0.4.5/splicekit/splicekit.config.template
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-06-30 14:19:54.000000 splicekit-0.4.5/splicekit/version
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-30 14:19:58.830692 splicekit-0.4.5/splicekit.egg-info/
--rw-rw-r--   0 rotg     (2023757) games       (20)    23915 2023-06-30 14:19:58.829232 splicekit-0.4.5/splicekit.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)      850 2023-06-30 14:19:58.829510 splicekit-0.4.5/splicekit.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-06-30 14:19:58.829771 splicekit-0.4.5/splicekit.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-09 07:35:55.000000 splicekit-0.4.5/splicekit.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)       62 2023-06-30 14:19:58.830357 splicekit-0.4.5/splicekit.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)       10 2023-06-30 14:19:58.830777 splicekit-0.4.5/splicekit.egg-info/top_level.txt
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.103729 splicekit-0.4.6/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    23915 2023-07-03 14:01:22.103334 splicekit-0.4.6/PKG-INFO
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    23517 2023-06-19 14:13:26.000000 splicekit-0.4.6/README.md
+-rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-07-03 14:01:22.103829 splicekit-0.4.6/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1150 2023-06-12 17:55:56.000000 splicekit-0.4.6/setup.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.087579 splicekit-0.4.6/splicekit/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    13844 2023-07-03 13:59:07.000000 splicekit-0.4.6/splicekit/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.090896 splicekit-0.4.6/splicekit/clusterlogfc/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5584 2023-05-05 11:49:03.000000 splicekit-0.4.6/splicekit/clusterlogfc/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.091634 splicekit-0.4.6/splicekit/config/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      951 2023-06-07 13:26:10.000000 splicekit-0.4.6/splicekit/config/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.101415 splicekit-0.4.6/splicekit/core/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      119 2023-06-20 11:22:13.000000 splicekit-0.4.6/splicekit/core/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     6667 2023-05-05 06:13:11.000000 splicekit-0.4.6/splicekit/core/anchors.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    16752 2023-05-24 07:18:50.000000 splicekit-0.4.6/splicekit/core/annotation.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-01-31 12:27:24.000000 splicekit-0.4.6/splicekit/core/delta_dar.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5407 2023-05-05 08:10:13.000000 splicekit-0.4.6/splicekit/core/exons.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    30130 2023-06-30 14:19:04.000000 splicekit-0.4.6/splicekit/core/features.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5662 2023-05-05 06:13:26.000000 splicekit-0.4.6/splicekit/core/genes.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1059 2023-06-07 14:32:33.000000 splicekit-0.4.6/splicekit/core/jbrowse2.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9033 2023-06-08 11:52:41.000000 splicekit-0.4.6/splicekit/core/jbrowse2_create.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2948 2023-04-26 12:12:45.000000 splicekit-0.4.6/splicekit/core/juan.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    18195 2023-06-21 14:33:41.000000 splicekit-0.4.6/splicekit/core/junctions.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    37713 2023-05-04 06:56:59.000000 splicekit-0.4.6/splicekit/core/motifs.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1663 2023-05-02 18:35:35.000000 splicekit-0.4.6/splicekit/core/patterns.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2420 2023-05-03 10:54:22.000000 splicekit-0.4.6/splicekit/core/promisc.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9045 2023-05-03 09:57:04.000000 splicekit-0.4.6/splicekit/core/report.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1527 2023-05-09 07:27:49.000000 splicekit-0.4.6/splicekit/folders.setup
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.102271 splicekit-0.4.6/splicekit/judge/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    26830 2023-06-08 11:49:08.000000 splicekit-0.4.6/splicekit/judge/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5402 2023-05-05 10:18:19.000000 splicekit-0.4.6/splicekit/splicecompare
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5117 2023-06-30 14:16:46.000000 splicekit-0.4.6/splicekit/splicekit
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1638 2023-06-06 07:56:19.000000 splicekit-0.4.6/splicekit/splicekit.config.template
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-07-03 14:00:08.000000 splicekit-0.4.6/splicekit/version
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-07-03 14:01:22.090456 splicekit-0.4.6/splicekit.egg-info/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    23915 2023-07-03 14:01:21.000000 splicekit-0.4.6/splicekit.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)      850 2023-07-03 14:01:21.000000 splicekit-0.4.6/splicekit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-07-03 14:01:21.000000 splicekit-0.4.6/splicekit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-09 07:35:55.000000 splicekit-0.4.6/splicekit.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) games       (20)       62 2023-07-03 14:01:21.000000 splicekit-0.4.6/splicekit.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)       10 2023-07-03 14:01:21.000000 splicekit-0.4.6/splicekit.egg-info/top_level.txt
```

### Comparing `splicekit-0.4.5/PKG-INFO` & `splicekit-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.4.5
+Version: 0.4.6
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `splicekit-0.4.5/README.md` & `splicekit-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/setup.py` & `splicekit-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/__init__.py` & `splicekit-0.4.6/splicekit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     folder_fname = os.path.join(core_path, "folders.setup")
     folders = open(folder_fname).read().split("\n")
     # create folders
     for folder_name in folders:
         if folder_name=="":
             continue
         os.system("mkdir -p {folder_name}".format(folder_name=folder_name))
-    print("[setup] Successfully setup splicekit v{version} analysis in {folder}\n".format(folder=os.getcwd(), version=core.current_version))
+    print("[setup] Successfully setup splicekit v{version} analysis in {folder}\n".format(folder=os.getcwd(), version=version))
 
 def clean():
     os.system("rm -f results/results_edgeR_junctions/*.tab > /dev/null 2>&1")
     os.system("rm -f jobs/jobs_edgeR_junctions/*.job > /dev/null 2>&1")
     os.system("rm -f results/results_edgeR_exons/*.tab > /dev/null 2>&1")
     os.system("rm -f jobs/jobs_edgeR_exons/*.job > /dev/null 2>&1")
```

### Comparing `splicekit-0.4.5/splicekit/clusterlogfc/__init__.py` & `splicekit-0.4.6/splicekit/clusterlogfc/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/config/__init__.py` & `splicekit-0.4.6/splicekit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/anchors.py` & `splicekit-0.4.6/splicekit/core/anchors.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/annotation.py` & `splicekit-0.4.6/splicekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/delta_dar.py` & `splicekit-0.4.6/splicekit/core/delta_dar.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/exons.py` & `splicekit-0.4.6/splicekit/core/exons.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/features.py` & `splicekit-0.4.6/splicekit/core/features.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/genes.py` & `splicekit-0.4.6/splicekit/core/genes.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/jbrowse2.py` & `splicekit-0.4.6/splicekit/core/jbrowse2.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/jbrowse2_create.py` & `splicekit-0.4.6/splicekit/core/jbrowse2_create.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/juan.py` & `splicekit-0.4.6/splicekit/core/juan.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/junctions.py` & `splicekit-0.4.6/splicekit/core/junctions.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/motifs.py` & `splicekit-0.4.6/splicekit/core/motifs.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/patterns.py` & `splicekit-0.4.6/splicekit/core/patterns.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/promisc.py` & `splicekit-0.4.6/splicekit/core/promisc.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/core/report.py` & `splicekit-0.4.6/splicekit/core/report.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/folders.setup` & `splicekit-0.4.6/splicekit/folders.setup`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/judge/__init__.py` & `splicekit-0.4.6/splicekit/judge/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/splicecompare` & `splicekit-0.4.6/splicekit/splicecompare`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/splicekit` & `splicekit-0.4.6/splicekit/splicekit`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit/splicekit.config.template` & `splicekit-0.4.6/splicekit/splicekit.config.template`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.5/splicekit.egg-info/PKG-INFO` & `splicekit-0.4.6/splicekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.4.5
+Version: 0.4.6
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `splicekit-0.4.5/splicekit.egg-info/SOURCES.txt` & `splicekit-0.4.6/splicekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*


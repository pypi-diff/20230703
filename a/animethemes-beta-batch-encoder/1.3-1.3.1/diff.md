# Comparing `tmp/animethemes-beta-batch-encoder-1.3.tar.gz` & `tmp/animethemes-beta-batch-encoder-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animethemes-beta-batch-encoder-1.3.tar", last modified: Mon Jul  3 04:42:14 2023, max compression
+gzip compressed data, was "animethemes-beta-batch-encoder-1.3.1.tar", last modified: Mon Jul  3 05:10:41 2023, max compression
```

## Comparing `animethemes-beta-batch-encoder-1.3.tar` & `animethemes-beta-batch-encoder-1.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 04:42:14.095469 animethemes-beta-batch-encoder-1.3/
--rw-rw-rw-   0        0        0     1082 2023-06-16 19:11:39.000000 animethemes-beta-batch-encoder-1.3/LICENSE
--rw-rw-rw-   0        0        0     5410 2023-07-03 04:42:14.094469 animethemes-beta-batch-encoder-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4502 2023-07-03 04:40:29.000000 animethemes-beta-batch-encoder-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 04:42:13.914469 animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/
--rw-rw-rw-   0        0        0     5410 2023-07-03 04:42:13.000000 animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-07-03 04:42:13.000000 animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 04:42:13.000000 animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-03 04:42:13.000000 animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-03 04:42:13.000000 animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 04:42:14.093488 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/
--rw-rw-rw-   0        0        0        0 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/__init__.py
--rw-rw-rw-   0        0        0     8114 2023-07-02 21:46:33.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/__main__.py
--rw-rw-rw-   0        0        0     1280 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_bitrate_mode.py
--rw-rw-rw-   0        0        0     2615 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_colorspace.py
--rw-rw-rw-   0        0        0    13543 2023-06-22 18:39:34.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_encode_webm.py
--rw-rw-rw-   0        0        0     4115 2023-06-22 08:05:47.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_encoding_config.py
--rw-rw-rw-   0        0        0     8234 2023-07-03 01:27:35.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_interface.py
--rw-rw-rw-   0        0        0     2527 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_loudnorm_filter.py
--rw-rw-rw-   0        0        0      779 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_seek.py
--rw-rw-rw-   0        0        0     5522 2023-07-03 04:36:38.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_seek_collector.py
--rw-rw-rw-   0        0        0     6594 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_source_file.py
--rw-rw-rw-   0        0        0     1375 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_utils.py
--rw-rw-rw-   0        0        0       42 2023-07-03 04:42:14.095469 animethemes-beta-batch-encoder-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-07-03 04:37:51.000000 animethemes-beta-batch-encoder-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 05:10:41.407932 animethemes-beta-batch-encoder-1.3.1/
+-rw-rw-rw-   0        0        0     1082 2023-06-16 19:11:39.000000 animethemes-beta-batch-encoder-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     5412 2023-07-03 05:10:41.406958 animethemes-beta-batch-encoder-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4502 2023-07-03 04:40:29.000000 animethemes-beta-batch-encoder-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 05:10:41.389923 animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/
+-rw-rw-rw-   0        0        0     5412 2023-07-03 05:10:41.000000 animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-07-03 05:10:41.000000 animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 05:10:41.000000 animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 05:10:41.000000 animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-03 05:10:41.000000 animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 05:10:41.404938 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/
+-rw-rw-rw-   0        0        0        0 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/__init__.py
+-rw-rw-rw-   0        0        0     8114 2023-07-02 21:46:33.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/__main__.py
+-rw-rw-rw-   0        0        0     1280 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_bitrate_mode.py
+-rw-rw-rw-   0        0        0     2615 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_colorspace.py
+-rw-rw-rw-   0        0        0    13543 2023-06-22 18:39:34.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_encode_webm.py
+-rw-rw-rw-   0        0        0     4115 2023-06-22 08:05:47.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_encoding_config.py
+-rw-rw-rw-   0        0        0     8234 2023-07-03 01:27:35.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_interface.py
+-rw-rw-rw-   0        0        0     2527 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_loudnorm_filter.py
+-rw-rw-rw-   0        0        0      779 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_seek.py
+-rw-rw-rw-   0        0        0     5486 2023-07-03 05:08:27.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_seek_collector.py
+-rw-rw-rw-   0        0        0     6594 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_source_file.py
+-rw-rw-rw-   0        0        0     1375 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-03 05:10:41.407932 animethemes-beta-batch-encoder-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2023-07-03 05:10:39.000000 animethemes-beta-batch-encoder-1.3.1/setup.py
```

### Comparing `animethemes-beta-batch-encoder-1.3/LICENSE` & `animethemes-beta-batch-encoder-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/PKG-INFO` & `animethemes-beta-batch-encoder-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-beta-batch-encoder
-Version: 1.3
+Version: 1.3.1
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `animethemes-beta-batch-encoder-1.3/README.md` & `animethemes-beta-batch-encoder-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/PKG-INFO` & `animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-beta-batch-encoder
-Version: 1.3
+Version: 1.3.1
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/SOURCES.txt` & `animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/__main__.py` & `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/__main__.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_bitrate_mode.py` & `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_bitrate_mode.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_colorspace.py` & `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_colorspace.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_encode_webm.py` & `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_encode_webm.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_encoding_config.py` & `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_encoding_config.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_interface.py` & `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_interface.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_loudnorm_filter.py` & `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_loudnorm_filter.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_seek.py` & `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_seek.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_seek_collector.py` & `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_seek_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
         len(x.strip()) == 0 \
         or all(SeekCollector.time_pattern.match(y) for y in x.split(',')) \
         and SeekCollector.start_positions in [len(x.split(',')), 0]
 
     validate_output_name = lambda _, x: \
         len(x.strip()) == 0 \
         or all(SeekCollector.filename_pattern.match(y) and not y.strip() in SeekCollector.all_output_names for y in x.split(',')) \
-        and SeekCollector.start_positions == len(x.split(',')) \
-        and len(set(x)) == len(x)
+        and SeekCollector.start_positions == len(x.split(',')) 
 
     def __init__(self, source_file):
         self.source_file = source_file
         self.start_positions = SeekCollector.prompt_time('Start time(s)')
         self.end_positions = SeekCollector.prompt_time('End time(s)')
         self.output_names = SeekCollector.prompt_output_name()
         self.new_audio_filters = SeekCollector.prompt_new_audio_filters(self)
```

### Comparing `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_source_file.py` & `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_source_file.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_utils.py` & `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_utils.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3/setup.py` & `animethemes-beta-batch-encoder-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='animethemes-beta-batch-encoder',
-    version='1.3',
+    version='1.3.1',
     author='AnimeThemes',
     author_email='admin@animethemes.moe',
     url='https://github.com/AnimeThemes/animethemes-batch-encoder',
     description='Generate/Execute FFmpeg commands for files in acting directory',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```


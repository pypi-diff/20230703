# Comparing `tmp/fajrGPT-1.3.tar.gz` & `tmp/fajrGPT-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.3.tar", last modified: Mon Jul  3 15:04:41 2023, max compression
+gzip compressed data, was "fajrGPT-1.3.1.tar", last modified: Mon Jul  3 18:52:06 2023, max compression
```

## Comparing `fajrGPT-1.3.tar` & `fajrGPT-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-03 15:04:41.781919 fajrGPT-1.3/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.3/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2944 2023-07-03 15:04:41.781752 fajrGPT-1.3/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.3/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-03 15:04:41.780734 fajrGPT-1.3/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.3/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.3/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    11596 2023-07-03 14:58:15.000000 fajrGPT-1.3/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-03 15:04:41.781588 fajrGPT-1.3/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2944 2023-07-03 15:04:41.000000 fajrGPT-1.3/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-03 15:04:41.000000 fajrGPT-1.3/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-03 15:04:41.000000 fajrGPT-1.3/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-03 15:04:41.000000 fajrGPT-1.3/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-03 15:04:41.000000 fajrGPT-1.3/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-03 15:04:41.000000 fajrGPT-1.3/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-03 15:04:41.781967 fajrGPT-1.3/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1127 2023-07-03 15:02:10.000000 fajrGPT-1.3/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-03 18:52:06.303242 fajrGPT-1.3.1/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.3.1/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-03 18:52:06.303099 fajrGPT-1.3.1/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.3.1/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-03 18:52:06.301882 fajrGPT-1.3.1/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.3.1/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.3.1/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    11596 2023-07-03 16:01:32.000000 fajrGPT-1.3.1/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-03 18:52:06.302883 fajrGPT-1.3.1/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-03 18:52:06.000000 fajrGPT-1.3.1/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-03 18:52:06.000000 fajrGPT-1.3.1/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-03 18:52:06.000000 fajrGPT-1.3.1/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-03 18:52:06.000000 fajrGPT-1.3.1/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-03 18:52:06.000000 fajrGPT-1.3.1/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-03 18:52:06.000000 fajrGPT-1.3.1/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-03 18:52:06.303284 fajrGPT-1.3.1/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-03 18:51:39.000000 fajrGPT-1.3.1/setup.py
```

### Comparing `fajrGPT-1.3/LICENSE` & `fajrGPT-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.3/PKG-INFO` & `fajrGPT-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.3
+Version: 1.3.1
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.3/README.md` & `fajrGPT-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.3/fajrGPT/quran_metadata.py` & `fajrGPT-1.3.1/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.3/fajrGPT/wake.py` & `fajrGPT-1.3.1/fajrGPT/wake.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
     # convert time to seconds
     countdown_seconds = convert_to_seconds(time)
 
     # Start countdown
     countdown(countdown_seconds)
 
-    # display a name of Allah
-    get_name_of_allah_and_explanation(names_flag)
-
     # Play audio with fade-in effect on a separate thread
     play_audio_thread = Thread(target=play_audio, args=(f'{output}.mp3',))
     play_audio_thread.start()
 
+    # display a name of Allah
+    get_name_of_allah_and_explanation(names_flag)
+
     # display the quran verses
     get_verses_and_explanations(countdown_seconds)
 
     # stop the audio once the user has completed reading the verses
     stop_audio()
 
     # return back to the main thread
```

### Comparing `fajrGPT-1.3/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.3.1/fajrGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.3
+Version: 1.3.1
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.3/setup.py` & `fajrGPT-1.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.3",
+    version="1.3.1",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```


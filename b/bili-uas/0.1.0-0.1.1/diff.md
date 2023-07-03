# Comparing `tmp/bili-uas-0.1.0.tar.gz` & `tmp/bili-uas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili-uas-0.1.0.tar", last modified: Sun Jul  2 23:40:09 2023, max compression
+gzip compressed data, was "bili-uas-0.1.1.tar", last modified: Mon Jul  3 09:19:19 2023, max compression
```

## Comparing `bili-uas-0.1.0.tar` & `bili-uas-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-02 23:40:09.992391 bili-uas-0.1.0/
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-02 23:40:09.985605 bili-uas-0.1.0/Bili_UAS/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.1.0/Bili_UAS/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1853 2023-06-30 11:05:14.000000 bili-uas-0.1.0/Bili_UAS/bili-config.py
--rw-r--r--   0 jhzg       (501) staff       (20)     5309 2023-06-30 11:49:14.000000 bili-uas-0.1.0/Bili_UAS/bili-live.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2831 2023-07-02 11:41:02.000000 bili-uas-0.1.0/Bili_UAS/bili-login.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2826 2023-06-30 11:05:14.000000 bili-uas-0.1.0/Bili_UAS/bili-user.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2510 2023-06-30 11:05:14.000000 bili-uas-0.1.0/Bili_UAS/bili-video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-02 23:40:09.987548 bili-uas-0.1.0/Bili_UAS/scripts/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.1.0/Bili_UAS/scripts/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2368 2023-06-30 11:28:07.000000 bili-uas-0.1.0/Bili_UAS/scripts/config.py
--rw-r--r--   0 jhzg       (501) staff       (20)     4271 2023-06-30 11:45:34.000000 bili-uas-0.1.0/Bili_UAS/scripts/live.py
--rw-r--r--   0 jhzg       (501) staff       (20)    10541 2023-06-30 11:05:14.000000 bili-uas-0.1.0/Bili_UAS/scripts/log_in.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1366 2023-06-30 11:05:14.000000 bili-uas-0.1.0/Bili_UAS/scripts/user.py
--rw-r--r--   0 jhzg       (501) staff       (20)     5687 2023-06-30 11:44:32.000000 bili-uas-0.1.0/Bili_UAS/scripts/video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-02 23:40:09.990127 bili-uas-0.1.0/Bili_UAS/utils/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.1.0/Bili_UAS/utils/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)    50101 2023-06-30 11:57:40.000000 bili-uas-0.1.0/Bili_UAS/utils/live_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2186 2023-06-30 10:59:22.000000 bili-uas-0.1.0/Bili_UAS/utils/search_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.1.0/Bili_UAS/utils/train_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    15374 2023-06-30 10:59:22.000000 bili-uas-0.1.0/Bili_UAS/utils/user_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-06-30 10:59:22.000000 bili-uas-0.1.0/Bili_UAS/utils/utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    18789 2023-06-30 10:59:22.000000 bili-uas-0.1.0/Bili_UAS/utils/video_utils.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-02 23:40:09.991253 bili-uas-0.1.0/Bili_UAS/writer/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.1.0/Bili_UAS/writer/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.1.0/Bili_UAS/writer/abnormal_monitor.py
--rw-r--r--   0 jhzg       (501) staff       (20)     3566 2023-06-30 10:59:22.000000 bili-uas-0.1.0/Bili_UAS/writer/log_writer.py
--rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.1.0/LICENSE
--rw-r--r--   0 jhzg       (501) staff       (20)     4583 2023-07-02 23:40:09.992249 bili-uas-0.1.0/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)     3880 2023-07-02 23:09:01.000000 bili-uas-0.1.0/README.md
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-02 23:40:09.992073 bili-uas-0.1.0/bili_uas.egg-info/
--rw-r--r--   0 jhzg       (501) staff       (20)     4583 2023-07-02 23:40:09.000000 bili-uas-0.1.0/bili_uas.egg-info/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)      808 2023-07-02 23:40:09.000000 bili-uas-0.1.0/bili_uas.egg-info/SOURCES.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-02 23:40:09.000000 bili-uas-0.1.0/bili_uas.egg-info/dependency_links.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      224 2023-07-02 23:40:09.000000 bili-uas-0.1.0/bili_uas.egg-info/entry_points.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      231 2023-07-02 23:40:09.000000 bili-uas-0.1.0/bili_uas.egg-info/requires.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-02 23:40:09.000000 bili-uas-0.1.0/bili_uas.egg-info/top_level.txt
--rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-02 23:40:09.992435 bili-uas-0.1.0/setup.cfg
--rw-r--r--   0 jhzg       (501) staff       (20)     1657 2023-07-02 23:33:24.000000 bili-uas-0.1.0/setup.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:19:19.174915 bili-uas-0.1.1/
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:19:19.168584 bili-uas-0.1.1/Bili_UAS/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.1.1/Bili_UAS/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1853 2023-06-30 11:05:14.000000 bili-uas-0.1.1/Bili_UAS/bili-config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     5309 2023-06-30 11:49:14.000000 bili-uas-0.1.1/Bili_UAS/bili-live.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2831 2023-07-02 11:41:02.000000 bili-uas-0.1.1/Bili_UAS/bili-login.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2826 2023-06-30 11:05:14.000000 bili-uas-0.1.1/Bili_UAS/bili-user.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2510 2023-06-30 11:05:14.000000 bili-uas-0.1.1/Bili_UAS/bili-video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:19:19.170149 bili-uas-0.1.1/Bili_UAS/scripts/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.1.1/Bili_UAS/scripts/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2368 2023-06-30 11:28:07.000000 bili-uas-0.1.1/Bili_UAS/scripts/config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4271 2023-06-30 11:45:34.000000 bili-uas-0.1.1/Bili_UAS/scripts/live.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    10541 2023-06-30 11:05:14.000000 bili-uas-0.1.1/Bili_UAS/scripts/log_in.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1366 2023-06-30 11:05:14.000000 bili-uas-0.1.1/Bili_UAS/scripts/user.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     5687 2023-06-30 11:44:32.000000 bili-uas-0.1.1/Bili_UAS/scripts/video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:19:19.172413 bili-uas-0.1.1/Bili_UAS/utils/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.1.1/Bili_UAS/utils/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    50101 2023-06-30 11:57:40.000000 bili-uas-0.1.1/Bili_UAS/utils/live_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2186 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/utils/search_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/utils/train_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    15374 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/utils/user_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/utils/utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    18789 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/utils/video_utils.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:19:19.173584 bili-uas-0.1.1/Bili_UAS/writer/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.1.1/Bili_UAS/writer/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/writer/abnormal_monitor.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     3566 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/writer/log_writer.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.1.1/LICENSE
+-rw-r--r--   0 jhzg       (501) staff       (20)     4605 2023-07-03 09:19:19.174758 bili-uas-0.1.1/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)     3880 2023-07-02 23:09:01.000000 bili-uas-0.1.1/README.md
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:19:19.174507 bili-uas-0.1.1/bili_uas.egg-info/
+-rw-r--r--   0 jhzg       (501) staff       (20)     4605 2023-07-03 09:19:19.000000 bili-uas-0.1.1/bili_uas.egg-info/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)      808 2023-07-03 09:19:19.000000 bili-uas-0.1.1/bili_uas.egg-info/SOURCES.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-03 09:19:19.000000 bili-uas-0.1.1/bili_uas.egg-info/dependency_links.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      224 2023-07-03 09:19:19.000000 bili-uas-0.1.1/bili_uas.egg-info/entry_points.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      229 2023-07-03 09:19:19.000000 bili-uas-0.1.1/bili_uas.egg-info/requires.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-03 09:19:19.000000 bili-uas-0.1.1/bili_uas.egg-info/top_level.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-03 09:19:19.174965 bili-uas-0.1.1/setup.cfg
+-rw-r--r--   0 jhzg       (501) staff       (20)     1958 2023-07-03 09:15:05.000000 bili-uas-0.1.1/setup.py
```

### Comparing `bili-uas-0.1.0/Bili_UAS/bili-config.py` & `bili-uas-0.1.1/Bili_UAS/bili-config.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/bili-live.py` & `bili-uas-0.1.1/Bili_UAS/bili-live.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/bili-login.py` & `bili-uas-0.1.1/Bili_UAS/bili-login.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/bili-user.py` & `bili-uas-0.1.1/Bili_UAS/bili-user.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/bili-video.py` & `bili-uas-0.1.1/Bili_UAS/bili-video.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/scripts/config.py` & `bili-uas-0.1.1/Bili_UAS/scripts/config.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/scripts/live.py` & `bili-uas-0.1.1/Bili_UAS/scripts/live.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/scripts/log_in.py` & `bili-uas-0.1.1/Bili_UAS/scripts/log_in.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/scripts/user.py` & `bili-uas-0.1.1/Bili_UAS/scripts/user.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/scripts/video.py` & `bili-uas-0.1.1/Bili_UAS/scripts/video.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/utils/live_utils.py` & `bili-uas-0.1.1/Bili_UAS/utils/live_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/utils/search_utils.py` & `bili-uas-0.1.1/Bili_UAS/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/utils/user_utils.py` & `bili-uas-0.1.1/Bili_UAS/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/utils/utils.py` & `bili-uas-0.1.1/Bili_UAS/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/utils/video_utils.py` & `bili-uas-0.1.1/Bili_UAS/utils/video_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/Bili_UAS/writer/log_writer.py` & `bili-uas-0.1.1/Bili_UAS/writer/log_writer.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/LICENSE` & `bili-uas-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/PKG-INFO` & `bili-uas-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.1.0
+Version: 0.1.1
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
-Keywords: BiliBili,auxiliary,analysis
+Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.9
```

### Comparing `bili-uas-0.1.0/README.md` & `bili-uas-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/bili_uas.egg-info/PKG-INFO` & `bili-uas-0.1.1/bili_uas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.1.0
+Version: 0.1.1
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
-Keywords: BiliBili,auxiliary,analysis
+Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.9
```

### Comparing `bili-uas-0.1.0/bili_uas.egg-info/SOURCES.txt` & `bili-uas-0.1.1/bili_uas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.0/setup.py` & `bili-uas-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
-with open('requirements.txt', "r") as f:
-    requirements = f.readlines()
+requirements = [
+    'bilibili-api-python~=15.5.1',
+    'setuptools~=68.0.0',
+    'wordcloud~=1.9.2',
+    'jieba~=0.42.1',
+    'scipy~=1.11.1',
+    'numpy~=1.25.0',
+    'tyro~=0.5.3',
+    'pandas~=2.0.3',
+    'tqdm~=4.65.0',
+    'matplotlib~=3.7.1',
+    'asyncio~=3.4.3',
+    'apscheduler~=3.10.1',
+    'requests~=2.31.0',
+    'httpx~=0.24.1']
 
 setup(
     name='bili-uas',
-    version='0.1.0',
+    version='0.1.1',
     license='GPLv3',
     author='jhzg',
     author_email='jhzg02200059@163.com',
     url='https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System',
     description='Assist up in personal, live, and video data analysis and prediction.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    keywords=["BiliBili", "auxiliary", "analysis"],
+    keywords=["BiliBili", "auxiliary", "analysis", "live", "video", "word_cloud"],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Topic :: Software Development :: Build Tools',
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)"
```


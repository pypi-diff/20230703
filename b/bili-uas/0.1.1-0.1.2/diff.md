# Comparing `tmp/bili-uas-0.1.1.tar.gz` & `tmp/bili-uas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili-uas-0.1.1.tar", last modified: Mon Jul  3 09:19:19 2023, max compression
+gzip compressed data, was "bili-uas-0.1.2.tar", last modified: Mon Jul  3 09:37:44 2023, max compression
```

## Comparing `bili-uas-0.1.1.tar` & `bili-uas-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:19:19.174915 bili-uas-0.1.1/
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:19:19.168584 bili-uas-0.1.1/Bili_UAS/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.1.1/Bili_UAS/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1853 2023-06-30 11:05:14.000000 bili-uas-0.1.1/Bili_UAS/bili-config.py
--rw-r--r--   0 jhzg       (501) staff       (20)     5309 2023-06-30 11:49:14.000000 bili-uas-0.1.1/Bili_UAS/bili-live.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2831 2023-07-02 11:41:02.000000 bili-uas-0.1.1/Bili_UAS/bili-login.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2826 2023-06-30 11:05:14.000000 bili-uas-0.1.1/Bili_UAS/bili-user.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2510 2023-06-30 11:05:14.000000 bili-uas-0.1.1/Bili_UAS/bili-video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:19:19.170149 bili-uas-0.1.1/Bili_UAS/scripts/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.1.1/Bili_UAS/scripts/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2368 2023-06-30 11:28:07.000000 bili-uas-0.1.1/Bili_UAS/scripts/config.py
--rw-r--r--   0 jhzg       (501) staff       (20)     4271 2023-06-30 11:45:34.000000 bili-uas-0.1.1/Bili_UAS/scripts/live.py
--rw-r--r--   0 jhzg       (501) staff       (20)    10541 2023-06-30 11:05:14.000000 bili-uas-0.1.1/Bili_UAS/scripts/log_in.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1366 2023-06-30 11:05:14.000000 bili-uas-0.1.1/Bili_UAS/scripts/user.py
--rw-r--r--   0 jhzg       (501) staff       (20)     5687 2023-06-30 11:44:32.000000 bili-uas-0.1.1/Bili_UAS/scripts/video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:19:19.172413 bili-uas-0.1.1/Bili_UAS/utils/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.1.1/Bili_UAS/utils/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)    50101 2023-06-30 11:57:40.000000 bili-uas-0.1.1/Bili_UAS/utils/live_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2186 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/utils/search_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/utils/train_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    15374 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/utils/user_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/utils/utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    18789 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/utils/video_utils.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:19:19.173584 bili-uas-0.1.1/Bili_UAS/writer/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.1.1/Bili_UAS/writer/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/writer/abnormal_monitor.py
--rw-r--r--   0 jhzg       (501) staff       (20)     3566 2023-06-30 10:59:22.000000 bili-uas-0.1.1/Bili_UAS/writer/log_writer.py
--rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.1.1/LICENSE
--rw-r--r--   0 jhzg       (501) staff       (20)     4605 2023-07-03 09:19:19.174758 bili-uas-0.1.1/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)     3880 2023-07-02 23:09:01.000000 bili-uas-0.1.1/README.md
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:19:19.174507 bili-uas-0.1.1/bili_uas.egg-info/
--rw-r--r--   0 jhzg       (501) staff       (20)     4605 2023-07-03 09:19:19.000000 bili-uas-0.1.1/bili_uas.egg-info/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)      808 2023-07-03 09:19:19.000000 bili-uas-0.1.1/bili_uas.egg-info/SOURCES.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-03 09:19:19.000000 bili-uas-0.1.1/bili_uas.egg-info/dependency_links.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      224 2023-07-03 09:19:19.000000 bili-uas-0.1.1/bili_uas.egg-info/entry_points.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      229 2023-07-03 09:19:19.000000 bili-uas-0.1.1/bili_uas.egg-info/requires.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-03 09:19:19.000000 bili-uas-0.1.1/bili_uas.egg-info/top_level.txt
--rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-03 09:19:19.174965 bili-uas-0.1.1/setup.cfg
--rw-r--r--   0 jhzg       (501) staff       (20)     1958 2023-07-03 09:15:05.000000 bili-uas-0.1.1/setup.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:37:44.929467 bili-uas-0.1.2/
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:37:44.924694 bili-uas-0.1.2/Bili_UAS/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.1.2/Bili_UAS/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1853 2023-07-03 09:35:16.000000 bili-uas-0.1.2/Bili_UAS/bili_config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     5309 2023-07-03 09:35:16.000000 bili-uas-0.1.2/Bili_UAS/bili_live.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2831 2023-07-03 09:35:16.000000 bili-uas-0.1.2/Bili_UAS/bili_login.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2826 2023-07-03 09:35:16.000000 bili-uas-0.1.2/Bili_UAS/bili_user.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2510 2023-07-03 09:35:16.000000 bili-uas-0.1.2/Bili_UAS/bili_video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:37:44.925989 bili-uas-0.1.2/Bili_UAS/scripts/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.1.2/Bili_UAS/scripts/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2368 2023-06-30 11:28:07.000000 bili-uas-0.1.2/Bili_UAS/scripts/config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4271 2023-06-30 11:45:34.000000 bili-uas-0.1.2/Bili_UAS/scripts/live.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    10541 2023-06-30 11:05:14.000000 bili-uas-0.1.2/Bili_UAS/scripts/log_in.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1366 2023-06-30 11:05:14.000000 bili-uas-0.1.2/Bili_UAS/scripts/user.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     5687 2023-06-30 11:44:32.000000 bili-uas-0.1.2/Bili_UAS/scripts/video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:37:44.927986 bili-uas-0.1.2/Bili_UAS/utils/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.1.2/Bili_UAS/utils/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    50101 2023-06-30 11:57:40.000000 bili-uas-0.1.2/Bili_UAS/utils/live_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2186 2023-06-30 10:59:22.000000 bili-uas-0.1.2/Bili_UAS/utils/search_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.1.2/Bili_UAS/utils/train_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    15374 2023-06-30 10:59:22.000000 bili-uas-0.1.2/Bili_UAS/utils/user_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-06-30 10:59:22.000000 bili-uas-0.1.2/Bili_UAS/utils/utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    18789 2023-06-30 10:59:22.000000 bili-uas-0.1.2/Bili_UAS/utils/video_utils.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:37:44.928515 bili-uas-0.1.2/Bili_UAS/writer/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.1.2/Bili_UAS/writer/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.1.2/Bili_UAS/writer/abnormal_monitor.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     3566 2023-06-30 10:59:22.000000 bili-uas-0.1.2/Bili_UAS/writer/log_writer.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.1.2/LICENSE
+-rw-r--r--   0 jhzg       (501) staff       (20)     4605 2023-07-03 09:37:44.929334 bili-uas-0.1.2/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)     3880 2023-07-02 23:09:01.000000 bili-uas-0.1.2/README.md
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-03 09:37:44.929151 bili-uas-0.1.2/bili_uas.egg-info/
+-rw-r--r--   0 jhzg       (501) staff       (20)     4605 2023-07-03 09:37:44.000000 bili-uas-0.1.2/bili_uas.egg-info/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)      808 2023-07-03 09:37:44.000000 bili-uas-0.1.2/bili_uas.egg-info/SOURCES.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-03 09:37:44.000000 bili-uas-0.1.2/bili_uas.egg-info/dependency_links.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-03 09:37:44.000000 bili-uas-0.1.2/bili_uas.egg-info/entry_points.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      229 2023-07-03 09:37:44.000000 bili-uas-0.1.2/bili_uas.egg-info/requires.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-03 09:37:44.000000 bili-uas-0.1.2/bili_uas.egg-info/top_level.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-03 09:37:44.929505 bili-uas-0.1.2/setup.cfg
+-rw-r--r--   0 jhzg       (501) staff       (20)     1960 2023-07-03 09:37:37.000000 bili-uas-0.1.2/setup.py
```

### Comparing `bili-uas-0.1.1/Bili_UAS/bili-config.py` & `bili-uas-0.1.2/Bili_UAS/bili_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Bili_UAS.bili-config
+Bili_UAS.bili_config
 
 This module provides a command line interface for setting work paths and danmu marks.
 """
 
 
 from __future__ import annotations
 from Bili_UAS.scripts import config as sc
```

### Comparing `bili-uas-0.1.1/Bili_UAS/bili-live.py` & `bili-uas-0.1.2/Bili_UAS/bili_live.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Bili_UAS.bili-live
+Bili_UAS.bili_live
 
 This module provides a command line interface for monitoring the live broadcast room and processing data
 """
 
 
 from __future__ import annotations
 from Bili_UAS.utils import live_utils as lu, user_utils as uu
```

### Comparing `bili-uas-0.1.1/Bili_UAS/bili-login.py` & `bili-uas-0.1.2/Bili_UAS/bili_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Bili_UAS.bili-login
+Bili_UAS.bili_login
 
 This module provides a command line interface for logining to bilibili.
 """
 
 
 from __future__ import annotations
 from Bili_UAS.scripts import log_in as sli, config as sc
```

### Comparing `bili-uas-0.1.1/Bili_UAS/bili-user.py` & `bili-uas-0.1.2/Bili_UAS/bili_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Bili_UAS.bili-user
+Bili_UAS.bili_user
 
 This module provides a command line interface for collecting user information and performing user operations.
 """
 
 
 from __future__ import annotations
 from Bili_UAS.utils import user_utils as uu
```

### Comparing `bili-uas-0.1.1/Bili_UAS/bili-video.py` & `bili-uas-0.1.2/Bili_UAS/bili_video.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Bili_UAS.bili-video
+Bili_UAS.bili_video
 
 This module provides a command line interface for downloading videos, audio or generating word image.
 """
 
 
 from __future__ import annotations
 import matplotlib.pyplot as plt
```

### Comparing `bili-uas-0.1.1/Bili_UAS/scripts/config.py` & `bili-uas-0.1.2/Bili_UAS/scripts/config.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/Bili_UAS/scripts/live.py` & `bili-uas-0.1.2/Bili_UAS/scripts/live.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/Bili_UAS/scripts/log_in.py` & `bili-uas-0.1.2/Bili_UAS/scripts/log_in.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/Bili_UAS/scripts/user.py` & `bili-uas-0.1.2/Bili_UAS/scripts/user.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/Bili_UAS/scripts/video.py` & `bili-uas-0.1.2/Bili_UAS/scripts/video.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/Bili_UAS/utils/live_utils.py` & `bili-uas-0.1.2/Bili_UAS/utils/live_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/Bili_UAS/utils/search_utils.py` & `bili-uas-0.1.2/Bili_UAS/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/Bili_UAS/utils/user_utils.py` & `bili-uas-0.1.2/Bili_UAS/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/Bili_UAS/utils/utils.py` & `bili-uas-0.1.2/Bili_UAS/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/Bili_UAS/utils/video_utils.py` & `bili-uas-0.1.2/Bili_UAS/utils/video_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/Bili_UAS/writer/log_writer.py` & `bili-uas-0.1.2/Bili_UAS/writer/log_writer.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/LICENSE` & `bili-uas-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/PKG-INFO` & `bili-uas-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.1.1
+Version: 0.1.2
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
 Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bili-uas-0.1.1/README.md` & `bili-uas-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.1/bili_uas.egg-info/PKG-INFO` & `bili-uas-0.1.2/bili_uas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.1.1
+Version: 0.1.2
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
 Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bili-uas-0.1.1/bili_uas.egg-info/SOURCES.txt` & `bili-uas-0.1.2/bili_uas.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 README.md
 setup.py
 Bili_UAS/__init__.py
-Bili_UAS/bili-config.py
-Bili_UAS/bili-live.py
-Bili_UAS/bili-login.py
-Bili_UAS/bili-user.py
-Bili_UAS/bili-video.py
+Bili_UAS/bili_config.py
+Bili_UAS/bili_live.py
+Bili_UAS/bili_login.py
+Bili_UAS/bili_user.py
+Bili_UAS/bili_video.py
 Bili_UAS/scripts/__init__.py
 Bili_UAS/scripts/config.py
 Bili_UAS/scripts/live.py
 Bili_UAS/scripts/log_in.py
 Bili_UAS/scripts/user.py
 Bili_UAS/scripts/video.py
 Bili_UAS/utils/__init__.py
```

### Comparing `bili-uas-0.1.1/setup.py` & `bili-uas-0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'asyncio~=3.4.3',
     'apscheduler~=3.10.1',
     'requests~=2.31.0',
     'httpx~=0.24.1']
 
 setup(
     name='bili-uas',
-    version='0.1.1',
+    version='0.1.2',
     license='GPLv3',
     author='jhzg',
     author_email='jhzg02200059@163.com',
     url='https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System',
     description='Assist up in personal, live, and video data analysis and prediction.',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -45,15 +45,15 @@
     package_data={'': ['*.txt', '*.md', 'LICENSE', 'setup.py', 'requirements.txt', '.gitignore']},
     exclude_package_data={'': ['test/*.py', 'test']},
     include_package_data=True,
     python_requires='>=3.9',
     install_requires=requirements,
     entry_points={
         'console_scripts': [
-            'bili_config = Bili_UAS.bili_config:tyro_cli',
-            'bili_live = Bili_UAS.bili_live:tyro_cli',
-            'bili_user = Bili_UAS.bili_user:tyro_cli',
-            'bili_video = Bili_UAS.bili_video:tyro_cli',
+            'bili-config = Bili_UAS.bili_config:tyro_cli',
+            'bili-live = Bili_UAS.bili_live:tyro_cli',
+            'bili-login = Bili_UAS.bili_login:tyro_cli',
+            'bili-video = Bili_UAS.bili_video:tyro_cli',
             'bili-user = Bili_UAS.bili_user:tyro_cli'
         ],
     }
 )
```


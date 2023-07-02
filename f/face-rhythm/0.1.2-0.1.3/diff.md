# Comparing `tmp/face_rhythm-0.1.2.tar.gz` & `tmp/face_rhythm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "face_rhythm-0.1.2.tar", last modified: Sun Jul  2 21:18:14 2023, max compression
+gzip compressed data, was "face_rhythm-0.1.3.tar", last modified: Sun Jul  2 22:57:27 2023, max compression
```

## Comparing `face_rhythm-0.1.2.tar` & `face_rhythm-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 21:18:14.268896 face_rhythm-0.1.2/
--rwxrwxrwx   0 root         (0) root         (0)       52 2022-12-06 23:48:14.000000 face_rhythm-0.1.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5990 2023-07-02 21:18:14.268589 face_rhythm-0.1.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5473 2022-12-14 16:31:29.000000 face_rhythm-0.1.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 21:18:14.266670 face_rhythm-0.1.2/face_rhythm/
--rwxrwxrwx   0 root         (0) root         (0)      488 2023-07-02 21:18:07.000000 face_rhythm-0.1.2/face_rhythm/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8633 2023-05-12 20:21:02.000000 face_rhythm-0.1.2/face_rhythm/data_importing.py
--rwxrwxrwx   0 root         (0) root         (0)    32078 2023-05-13 04:09:53.000000 face_rhythm-0.1.2/face_rhythm/decomposition.py
--rwxrwxrwx   0 root         (0) root         (0)    11685 2023-05-12 00:14:16.000000 face_rhythm-0.1.2/face_rhythm/h5_handling.py
--rwxrwxrwx   0 root         (0) root         (0)   126521 2023-07-02 21:07:53.000000 face_rhythm-0.1.2/face_rhythm/helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    30187 2023-07-02 14:05:50.000000 face_rhythm-0.1.2/face_rhythm/point_tracking.py
--rwxrwxrwx   0 root         (0) root         (0)     3460 2023-07-02 17:54:14.000000 face_rhythm-0.1.2/face_rhythm/project.py
--rwxrwxrwx   0 root         (0) root         (0)    67492 2023-07-02 00:34:16.000000 face_rhythm-0.1.2/face_rhythm/rois.py
--rwxrwxrwx   0 root         (0) root         (0)    14562 2023-05-13 02:35:47.000000 face_rhythm-0.1.2/face_rhythm/spectral_analysis.py
--rwxrwxrwx   0 root         (0) root         (0)    41698 2023-07-02 17:53:13.000000 face_rhythm-0.1.2/face_rhythm/util.py
--rwxrwxrwx   0 root         (0) root         (0)    31210 2023-05-13 02:22:13.000000 face_rhythm-0.1.2/face_rhythm/visualization.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 21:18:14.268132 face_rhythm-0.1.2/face_rhythm.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5990 2023-07-02 21:18:14.000000 face_rhythm-0.1.2/face_rhythm.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      454 2023-07-02 21:18:14.000000 face_rhythm-0.1.2/face_rhythm.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-02 21:18:14.000000 face_rhythm-0.1.2/face_rhythm.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       12 2023-07-02 21:18:14.000000 face_rhythm-0.1.2/face_rhythm.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-02 21:18:14.269014 face_rhythm-0.1.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2995 2023-07-02 21:12:13.000000 face_rhythm-0.1.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 22:57:27.638813 face_rhythm-0.1.3/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2022-12-06 23:48:14.000000 face_rhythm-0.1.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5990 2023-07-02 22:57:27.638597 face_rhythm-0.1.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5473 2022-12-14 16:31:29.000000 face_rhythm-0.1.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 22:57:27.637020 face_rhythm-0.1.3/face_rhythm/
+-rwxrwxrwx   0 root         (0) root         (0)      488 2023-07-02 22:57:00.000000 face_rhythm-0.1.3/face_rhythm/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8633 2023-05-12 20:21:02.000000 face_rhythm-0.1.3/face_rhythm/data_importing.py
+-rwxrwxrwx   0 root         (0) root         (0)    32078 2023-05-13 04:09:53.000000 face_rhythm-0.1.3/face_rhythm/decomposition.py
+-rwxrwxrwx   0 root         (0) root         (0)    11685 2023-05-12 00:14:16.000000 face_rhythm-0.1.3/face_rhythm/h5_handling.py
+-rwxrwxrwx   0 root         (0) root         (0)   126521 2023-07-02 21:07:53.000000 face_rhythm-0.1.3/face_rhythm/helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    30187 2023-07-02 14:05:50.000000 face_rhythm-0.1.3/face_rhythm/point_tracking.py
+-rwxrwxrwx   0 root         (0) root         (0)     3405 2023-07-02 22:46:47.000000 face_rhythm-0.1.3/face_rhythm/project.py
+-rwxrwxrwx   0 root         (0) root         (0)    67492 2023-07-02 00:34:16.000000 face_rhythm-0.1.3/face_rhythm/rois.py
+-rwxrwxrwx   0 root         (0) root         (0)    14562 2023-05-13 02:35:47.000000 face_rhythm-0.1.3/face_rhythm/spectral_analysis.py
+-rwxrwxrwx   0 root         (0) root         (0)    41698 2023-07-02 17:53:13.000000 face_rhythm-0.1.3/face_rhythm/util.py
+-rwxrwxrwx   0 root         (0) root         (0)    31210 2023-05-13 02:22:13.000000 face_rhythm-0.1.3/face_rhythm/visualization.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 22:57:27.638222 face_rhythm-0.1.3/face_rhythm.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5990 2023-07-02 22:57:27.000000 face_rhythm-0.1.3/face_rhythm.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      454 2023-07-02 22:57:27.000000 face_rhythm-0.1.3/face_rhythm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-02 22:57:27.000000 face_rhythm-0.1.3/face_rhythm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       12 2023-07-02 22:57:27.000000 face_rhythm-0.1.3/face_rhythm.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-02 22:57:27.638898 face_rhythm-0.1.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2995 2023-07-02 21:12:13.000000 face_rhythm-0.1.3/setup.py
```

### Comparing `face_rhythm-0.1.2/PKG-INFO` & `face_rhythm-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: face_rhythm
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pipeline for analysis of facial behavior using optical flow
 Home-page: https://github.com/RichieHakim/face-rhythm
 Author: Rich Hakim
 Keywords: face beahvior optical flow
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `face_rhythm-0.1.2/README.md` & `face_rhythm-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.2/face_rhythm/data_importing.py` & `face_rhythm-0.1.3/face_rhythm/data_importing.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.2/face_rhythm/decomposition.py` & `face_rhythm-0.1.3/face_rhythm/decomposition.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.2/face_rhythm/h5_handling.py` & `face_rhythm-0.1.3/face_rhythm/h5_handling.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.2/face_rhythm/helpers.py` & `face_rhythm-0.1.3/face_rhythm/helpers.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.2/face_rhythm/point_tracking.py` & `face_rhythm-0.1.3/face_rhythm/point_tracking.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.2/face_rhythm/project.py` & `face_rhythm-0.1.3/face_rhythm/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         """
         Creates a config.yaml file.
         """
         contents_basic = {
             'general': {
                 'date_created': datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                 'date_modified': datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
-                'system_versions': util.system_info(),
                 'path_created': path_config,
             },
             'paths': {
                 'project': directory_project,
                 'config': path_config,
                 'run_info': path_run_info,
             },
```

### Comparing `face_rhythm-0.1.2/face_rhythm/rois.py` & `face_rhythm-0.1.3/face_rhythm/rois.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.2/face_rhythm/spectral_analysis.py` & `face_rhythm-0.1.3/face_rhythm/spectral_analysis.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.2/face_rhythm/util.py` & `face_rhythm-0.1.3/face_rhythm/util.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.2/face_rhythm/visualization.py` & `face_rhythm-0.1.3/face_rhythm/visualization.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.2/face_rhythm.egg-info/PKG-INFO` & `face_rhythm-0.1.3/face_rhythm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: face-rhythm
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pipeline for analysis of facial behavior using optical flow
 Home-page: https://github.com/RichieHakim/face-rhythm
 Author: Rich Hakim
 Keywords: face beahvior optical flow
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `face_rhythm-0.1.2/setup.py` & `face_rhythm-0.1.3/setup.py`

 * *Files identical despite different names*


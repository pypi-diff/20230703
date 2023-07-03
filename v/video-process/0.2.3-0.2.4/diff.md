# Comparing `tmp/video_process-0.2.3.tar.gz` & `tmp/video_process-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_process-0.2.3.tar", max compression
+gzip compressed data, was "video_process-0.2.4.tar", max compression
```

## Comparing `video_process-0.2.3.tar` & `video_process-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      453 2023-07-03 07:20:58.460116 video_process-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      125 2023-06-28 09:02:50.789446 video_process-0.2.3/video_process/__init__.py
--rw-r--r--   0        0        0     5517 2023-06-29 03:51:51.970247 video_process-0.2.3/video_process/graph_builder.py
--rwxr-xr-x   0        0        0     1464 2023-06-29 06:24:47.835149 video_process-0.2.3/video_process/index.py
--rw-r--r--   0        0        0     1685 2023-06-21 08:58:19.044108 video_process-0.2.3/video_process/lib.py
--rw-r--r--   0        0        0     1134 2023-06-28 08:59:43.686218 video_process-0.2.3/video_process/subtitle.py
--rw-r--r--   0        0        0     4074 2023-07-03 07:20:37.997715 video_process-0.2.3/video_process/utils.py
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      453 2023-07-03 08:39:18.432091 video_process-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      167 2023-07-03 08:37:18.348712 video_process-0.2.4/video_process/__init__.py
+-rw-r--r--   0        0        0     5517 2023-06-29 03:51:51.970247 video_process-0.2.4/video_process/graph_builder.py
+-rwxr-xr-x   0        0        0     1464 2023-06-29 06:24:47.835149 video_process-0.2.4/video_process/index.py
+-rw-r--r--   0        0        0     1741 2023-07-03 08:37:13.109063 video_process-0.2.4/video_process/lib.py
+-rw-r--r--   0        0        0     1134 2023-06-28 08:59:43.686218 video_process-0.2.4/video_process/subtitle.py
+-rw-r--r--   0        0        0     4074 2023-07-03 07:20:37.997715 video_process-0.2.4/video_process/utils.py
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.2.4/PKG-INFO
```

### Comparing `video_process-0.2.3/video_process/graph_builder.py` & `video_process-0.2.4/video_process/graph_builder.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.3/video_process/index.py` & `video_process-0.2.4/video_process/index.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.3/video_process/lib.py` & `video_process-0.2.4/video_process/lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,9 +44,10 @@
     response = client.upload_file(
         Bucket=BUCKET_NAME,
         LocalFilePath=file_path,
         Key=key,
         PartSize=10,
         MAXThread=10,
         EnableMD5=False,
+        Metadata={"Content-Disposition": "attachment"},
     )
     return response["ETag"]
```

### Comparing `video_process-0.2.3/video_process/subtitle.py` & `video_process-0.2.4/video_process/subtitle.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.3/video_process/utils.py` & `video_process-0.2.4/video_process/utils.py`

 * *Files identical despite different names*


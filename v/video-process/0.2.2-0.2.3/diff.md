# Comparing `tmp/video_process-0.2.2.tar.gz` & `tmp/video_process-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_process-0.2.2.tar", max compression
+gzip compressed data, was "video_process-0.2.3.tar", max compression
```

## Comparing `video_process-0.2.2.tar` & `video_process-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      453 2023-07-03 06:59:40.542560 video_process-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      125 2023-06-28 09:02:50.789446 video_process-0.2.2/video_process/__init__.py
--rw-r--r--   0        0        0     5517 2023-06-29 03:51:51.970247 video_process-0.2.2/video_process/graph_builder.py
--rwxr-xr-x   0        0        0     1464 2023-06-29 06:24:47.835149 video_process-0.2.2/video_process/index.py
--rw-r--r--   0        0        0     1685 2023-06-21 08:58:19.044108 video_process-0.2.2/video_process/lib.py
--rw-r--r--   0        0        0     1134 2023-06-28 08:59:43.686218 video_process-0.2.2/video_process/subtitle.py
--rw-r--r--   0        0        0     3890 2023-07-03 07:10:18.629501 video_process-0.2.2/video_process/utils.py
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      453 2023-07-03 07:20:58.460116 video_process-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-06-28 09:02:50.789446 video_process-0.2.3/video_process/__init__.py
+-rw-r--r--   0        0        0     5517 2023-06-29 03:51:51.970247 video_process-0.2.3/video_process/graph_builder.py
+-rwxr-xr-x   0        0        0     1464 2023-06-29 06:24:47.835149 video_process-0.2.3/video_process/index.py
+-rw-r--r--   0        0        0     1685 2023-06-21 08:58:19.044108 video_process-0.2.3/video_process/lib.py
+-rw-r--r--   0        0        0     1134 2023-06-28 08:59:43.686218 video_process-0.2.3/video_process/subtitle.py
+-rw-r--r--   0        0        0     4074 2023-07-03 07:20:37.997715 video_process-0.2.3/video_process/utils.py
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.2.3/PKG-INFO
```

### Comparing `video_process-0.2.2/video_process/graph_builder.py` & `video_process-0.2.3/video_process/graph_builder.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.2/video_process/index.py` & `video_process-0.2.3/video_process/index.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.2/video_process/lib.py` & `video_process-0.2.3/video_process/lib.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.2/video_process/subtitle.py` & `video_process-0.2.3/video_process/subtitle.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.2/video_process/utils.py` & `video_process-0.2.3/video_process/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,29 +37,32 @@
     download_file(video_url, video_path)
     data["video_path"] = video_path
 
     if data.get("enable_bg"):
         bg = data["bg"]
         if bg["bg_type"] == "video" and bg.get("bg_video_url"):
             video_url = bg["bg_video_url"]
-            video_path = os.path.join(base_dir, "bg_video.mp4")
+            extension = get_file_extension(video_url)
+            video_path = os.path.join(base_dir, "bg_video{extension}")
             download_file(video_url, video_path)
             bg["bg_video_path"] = video_path
         elif bg["bg_type"] == "image" and bg.get("bg_image_url"):
             image_url = bg["bg_image_url"]
-            image_path = os.path.join(base_dir, "bg_image.jpg")
+            extension = get_file_extension(image_url)
+            image_path = os.path.join(base_dir, "bg_image{extension}")
             download_file(image_url, image_path)
             bg["bg_image_path"] = image_path
 
     # 处理背景音乐字段
     if data.get("enable_bgm"):
         bg_music = data["bgm"]
         if bg_music.get("bgm_url"):
             music_url = bg_music["bgm_url"]
-            music_path = os.path.join(base_dir, "bg_music.mp3")
+            extension = get_file_extension(music_url)
+            music_path = os.path.join(base_dir, f"bg_music{extension}")
             download_file(music_url, music_path)
             bg_music["path"] = music_path
 
     # 处理字幕字段
     if data.get("enable_subtitle"):
         subtitle = data["subtitle"]
         if subtitle.get("url"):
```

